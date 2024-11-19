pipeline{
    agent{
        label " java-slave"
    }
    stages{
        stage("Build"){
            steps{
                retry(3){
                    echo "welcome to jenkins pipelin"
                    error"printing the error message"
                }
            }
        }
    }
}
