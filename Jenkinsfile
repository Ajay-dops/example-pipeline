pipeline{
    agent{
        label "java-slave"
    }
    stages{
        stage("Build"){
             
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
    }
}
