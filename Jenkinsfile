pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('Checkout'){
            steps{
                git branch: 'master', url: 'https://github.com/machredd/SpringPetClinic.git'
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
bat 'Java -jar C:/Program Files/Jenkins/workspace/SpringPetClinic/target/spring-petclinic-2.1.0Build-SHAPSHOT.jar'
        
        }
    }
}
}
