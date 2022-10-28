 pipeline{
        agent any
//        stages{
//            stage('Clone'){
//                steps{
//                    sh "https://github.com/Libz4/ToDo-WebApp.git"
//                }
//            }


            stage('Copy Files & Folders'){
                steps{
                    sh "cp app.py /home/azureuser/ToDoWA"
                    sh "cp requirements.txt /home/azureuser/ToDoWA"
                    sh "cp -r /home/jenkins/.jenkins/workspace/ToDo-WebApp/instance /home/azureuser/ToDoWA"
                    sh "cp -r /home/jenkins/.jenkins/workspace/ToDo-WebApp/__pycache__/ /home/azureuser/ToDoWA"
                    sh "cp -r /home/jenkins/.jenkins/workspace/ToDo-WebApp/templates/ /home/azureuser/ToDoWA"
                    sh "cp -r /home/jenkins/.jenkins/workspace/ToDo-WebApp/venv/ /home/azureuser/ToDoWA"
                }
            }



            stage('Navigate to Project dir'){
                steps{
                    sh "cd /home/azureuser/ToDoWA"
                }
            }



            stage('Build Docker') {
                steps{
                    sh "docker build -t flask-app /home/azureuser/ToDoWA"
                }
            }
            stage("run docker container"){
                steps{
                    sh "docker run -p 5000:5000 --name flask-app -d flask-app "
                }
            }
        }
}
