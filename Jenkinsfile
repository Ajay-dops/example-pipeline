 pipeline{
    agent{
        label " java-slave"
    }
    environment{
        NAME = "ajay"
        JOB = " DevOps "
    }
    stages{
        stage("build"){
            environment{
                NAME = "Srinu"//presedence //
                echo " printing my name ${NAME} "
                echo " prinitng my job ${JOB}"
            }
        }
    }
 }
