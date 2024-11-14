pipeline {
    agent {
        label 'java-node'
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
