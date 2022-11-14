pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
             echo 'Build'
             sh 'mvn clean package'
            }
        }
        stage('Test'){
            steps{
              echo 'Test'
              sh 'mvn test'
            }
        }
       
        stage('Push to atrifactory'){
            steps{
                echo 'Build'
            }
        }


        stage('Deploy to Dev'){
            steps{
                 echo 'Deploy Dev'
            }
        }
        stage('Deploy to QA'){
            steps{
                 echo 'Deploy QA'
            }
        }
        
         stage('Deploy to Staging'){
            steps{
                echo 'Deploy Stage'
            }
        }
         stage('Deploy to Prod'){
            steps{
               echo 'Deploy Prod'
            } 
        }

        
    }
    post{
            failure{
                echo 'fail'
            }
            
            success{
                echo 'Success'
            }
            
           
        }
} 