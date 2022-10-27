pipeline{
        agent any
        stages{
            stage('Clone'){
                steps{
                    sh "git clone https://github.com/Libz4/ToDo-WebApp.git"
                }
            }  
         stage('build'){
                steps{
                    sh "python3 app.py"        
                }
            }  
         stage('test'){
                steps{
                    sh "python3 -m pytest --cov"    
                        
                }
            }
         tage('deploy'){
                steps{
                    sh "python3 -m pytest --cov"    
                        
                }
            }             
        }
}

