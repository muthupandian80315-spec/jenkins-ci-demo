pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'chmod +x test.sh'
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/index.html'
            }
        }
    }
}

