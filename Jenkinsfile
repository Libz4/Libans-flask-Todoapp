 pipeline{
        agent any
        stages{
            stage('Clone'){
                steps{
                    sh "https://github.com/Libz4/ToDo-WebApp.git"
                }
            }


            stage('copy files'){
                steps{
                    sh "cp app.py /home/jenkins/.jenkins/workspace/ToDo-WebApp"
                    sh "cp requirements.txt /home/jenkins/.jenkins/workspace/ToDo-WebApp"
                    sh "cp -r /home/jenkins/.jenkins/workspace/ToDo-WebApp"
                }
            }



            stage('change foler to home'){
                steps{
                    sh "cd /home/jenkins/.jenkins/workspace/ToDo-WebApp"
                }
            }



            stage('Build Docker') {
                steps{
                    sh "docker build -t flask-app /home/jenkins/.jenkins/workspace/ToDo-WebApp"
                }
            }
            stage("run docker container"){
                steps{
                    sh "docker run -p 5000:5000 --name flask-app -d flask-app "
                }
            }
        }
}
