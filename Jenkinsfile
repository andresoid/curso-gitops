pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Build') {
            agent { label 'docker-agent'}
            steps {
                sh '''
                    echo "con contenedor docker"
                    ls -la /
                '''
            }
        }
    }
}
