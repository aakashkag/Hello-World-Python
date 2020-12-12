
pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Setup') {
            steps {
                echo 'Setup Stage'
                sh """
                    PATH=${PATH}:/usr/bin
          		    pip3 install -r requirements.txt
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

