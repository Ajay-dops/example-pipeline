pipeline{
    agent{
        label "java-label"
    }
    parameters{
        choice(name: 'deployToprod', 
            choices: ['yes','no'],
            description: 'Deploy to prodccution'
            )
    }
    stages{
        stage("build"){
            steps{
                echo "building the application"
            }
        }
        stage("deploy to prod"){
            when {
                expression{
                    params.deployToprod == 'yes'
                }
            }
        }
    }

}
