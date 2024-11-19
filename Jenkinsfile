pipeline{
    agent{
        label "java-slave"
    }
    stages{
        stage(build){
            steps{
                sh " docker pull nginx"
            }
        }
    }
}
