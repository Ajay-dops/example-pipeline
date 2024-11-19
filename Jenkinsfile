pipeline{
    agent{
        label "java-slave"
    }
    stages{
        stage(build){
            steps{
                sh " hostname -i"
            }
        }
    }
}
