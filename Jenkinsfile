pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Hello'){
            steps {
                echo "Hello world"
                sh 'date'
                echo "executing my first stage"
            }
        }
    }
}
