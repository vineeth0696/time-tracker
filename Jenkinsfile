pipeline{
    agent any
     tools{
        maven 'maven 3.8.6'
    }
    stages{
        stage('Git Clone'){
            steps{
                git 'https://github.com/Msocial123/time-tracker.git'
            }
        }
         stage('Maven Build'){
            steps{
               sh 'mvn package'
            }
        }
         stage('Maven Test'){
             steps{
                sh 'mvn test'
             }
         }
         stage('Deploy'){
             steps{
                 echo "Sucessfully Deployed Project"
             }
         }
    }
}
