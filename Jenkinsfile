
pipeline {
    agent any 
    stages {
        stage('Setup') {
            steps {
                echo 'Setup Stage'
                sh """
          		    pip install -r requirements.txt
          	     """ 
            }
        }
        stage('Build') {
            steps {
                echo 'Build Stage'
            }
        }
        stage('QA') {
            steps {
                echo 'QA Stage' 
            }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy Stage' 
            }
        }
         stage('Monitor') {
            steps {
                echo 'Monitor Stage' 
            }
        }
    }
}

