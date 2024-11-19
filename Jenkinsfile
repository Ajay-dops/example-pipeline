pipeline{
    agent{
        label "java-slave"
    }
    stages{
        stage("Build"){
            steps{
                timeout (time:5, unit: SECONDS){
                    echo " sleeping for 1 min"
                    sleep 60
                }
            }
        }
    }
 
