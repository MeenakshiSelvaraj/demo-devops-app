pipeline {
    agent any

    tools {
        maven 'Maven'
    }

        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }
    }
}
