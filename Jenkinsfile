pipeline {
    agent any

    stages {

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

        stage('Run Container') {
    steps {
        sh 'docker run -d -p 8085:8080 demo-app'
    }
}
    }
}
