pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('Checkout'){
            steps{
                git branch: 'master', url: ''
            }
        }
        stage('Build'){
            tools{
                jdk 'JAVA_HOME'
            }
            steps{
                bat 'mvn compile'
            }
        }
        stage('Package'){
            tools{
                jdk 'JAVA_HOME'
            }
            steps{
                bat 'mvn package'
            }
        }
         stage('Deploy'){
      steps{
bat 'Java -jar C:/Program Files/Jenkins/workspace/ecommercebeckend/target/ecommercebackend-0.0.1-SHAPSHOT.jar'
        
        }
    }
}
}
