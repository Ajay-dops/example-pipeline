pipeline{
    agent{
        label "java-slave"
    }
    stages{
        stage("Build"){
            steps{
               echo "building the project"
            }
             
        }
        stage('Scans'){
            parallel{
                stage('Sonar'){
                    steps{
                    echo 'running sonar scan'
                    sleep 10
                    }
                }
                stage('checkmarx'){
                    steps{
                        echo 'running checkmarx scan'
                        sleep 10
                    }
                }
                stage('contrast'){
                    steps{
                        echo " running constrant scan"
                        sleep 10
                    }
                } 
            }
        }
        stage('deploy'){
            steps{
                echo " deploying the project"
            }
        }
    }
}
