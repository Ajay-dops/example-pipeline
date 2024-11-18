pipeline{
    agent{
        label 'java-slave'
    }
    stages{
        stage("hello"){
            steps{
            echo"printing hello"
            }
        }
        stage('scriptblock'){
            steps{
                script{
                def course = "jenkins"
                if (course == "k8s")
                 println("thanks for enrolling in k8s")
                else
                 println("do learn")
                }
            }
        }
    }
}
