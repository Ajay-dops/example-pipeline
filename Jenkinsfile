 pipeline{
    agent{
        label "java-slave"
    }
    environment{
        DEVOPS_CREDS = credentials ("dockerhub_creds")
    }
    stages{
        stage("DockerBP"){
            steps{
                sh "Docker pull nginx"
                echo " printing images before changing the tag"
                sh " Docker images"
                sh " Docker tag nginx ajaydops/nginx:b5"
                echo " priting images after changing the tag"
                sh " Docker images"
                echo " Dcoker login"
                sh " docker login -u ${DEVOPS_CREDS_USR} -p ${DEVOPS_CREDS_PSW}"
                echo " pusing the image to repo"
                sh " docker push ajaydops/nginx:b5 "
            
                

            }
        }
        }
    }
 }
