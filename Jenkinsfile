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
                    branch  "main|master"
            }
            steps{
                echo " deploying to stg"
            }
        }
    }
}
