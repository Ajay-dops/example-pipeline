pipeline{
    agent{
        label "java-slave"
    }
    environment{
        DEPLOY_TO = "production"
    }
    stages{
        stage("Build"){
            steps{
                echo " Building the project"
            }
        }
        stage("sonar"){
            steps{
                echo " running the sonar"
            }
        }
        stage("Deploy to stg"){
            when{
                expression{
                    env.BRANCH_NAME ==~/(production|staging|main)/
                } 
            }
            steps{
                echo " deploying to stg"
            }
        }
        stage(" Deploy to prod"){
            when {
                allOf{
                    branch 'main'
                    environment name: "DEPLOY_TO", value: "production"
                }
            }
            steps{
                echo " Deploying to prod"
            }
        }
    }
}
