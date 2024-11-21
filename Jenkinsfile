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
                    BRANCH_NAME == /(production|staging)/
                } 
            }
            steps{
                echo " deploying to stg"
            }
        }
    }
}
