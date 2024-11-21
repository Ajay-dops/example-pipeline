pipeline{
    agent{
        label "java-slave"
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
            steps{
                echo "deploying to production"
            }
        }
    }

}
