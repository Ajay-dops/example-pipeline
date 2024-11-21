pipeline{
    agent{
        label "java-slave"
    }
    parameters{
        string (name: 'PERSON', defaultvalue: 'siva', description: 'Enter your name')
        choice (name: 'COURSE', choices: ['k8s', 'jenkins','docker'], description: 'select the course')
        booleanParam (name: 'CLOUD', defaultvalue: true, description: 'do you want to learn')
    }
    environment{
        CI_SERVER = 'jenkins'
    }
    stages{
        stage('Firststage'){
            steps{
                echo " welcome ${params.PERSON}"
                echo " you enrolled for ${params.COURSE}"
                echo " you want to learn in ${params.CLOUD}"
                echo "you are using ${CI_SERVER}"
            }
        }
    }
}
