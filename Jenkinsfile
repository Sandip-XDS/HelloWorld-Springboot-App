pipeline{
    
    agent any
    stages{
        
        stage('GitClone'){
            steps{
                git 'https://github.com/Sandip-XDS/HelloWorld-Springboot-App.git'
            }
        }
        
        stage('Maven_Test'){
            steps{
                sh 'mvn test'
            }
        }

        stage('Maven_Build'){
            steps{
                sh 'mvn package'
            }
        }

        stage('Maven_Deploy'){
            steps{
                echo "Deploying the war file to the Server"
            }
        }


        
    }
    
}
