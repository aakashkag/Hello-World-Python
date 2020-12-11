
pipeline {
    agent any 
    stages {
        stage('Setup') {
            steps {
                echo 'Setup Stage'
                sh """
                    PATH=${PATH}:/usr/local/bin
          		    pip install -r requirements.txt
          	     """ 
            }
        }
        stage('Build') {
            steps {
                echo 'Build Stage'
                sh 'python helloworld.py'
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

