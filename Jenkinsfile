 pipeline{
    agent{
        label "java-slave"
    }
    environment{
        NAME = "ajay"
        COURSE = "devops"

    }
    stages{
        stage("Build"){
            environment{
                CLOUD = "gcp"
            }
            steps{
                echo " welcome ${NAME}"
                echo " you enrolled for ${COURSE} course"
                echo " you are certified in ${CLOUD}"
            }
        }
    }
 }
