 pipeline{
    agent{
        label " java-slave"
    }
    environment{
        NAME = "Ajay"
        COUNTRY = "India"
    }
    stages{
        stage("Build"){
            environment{
                LOCATION = "USA"
            }
            steps{
                echo "your ${NAME}"
                echo "which ${COUNTRY}"
                echo " your current ${LOCATION}"
            }
        }
    }
 }
