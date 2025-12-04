pipeline{
    agent any{
        stages{
            stage('Build'){
                steps{
                    echo "Build docker image"
                    bat "docker build -t image:/v1"
                }
            }
            stage('Push'){
                steps{
                    bat "docker push image:"
                }
            }
            stage('login'){
                steps{
                    bat "docker login -u -p"
                }
            }
            stage('Run'){
                steps{
                    bat "docker run "
                }
            }
        }
    }
}