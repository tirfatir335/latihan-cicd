pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Mengambil kode dari GitHub...'
            }
        }
        stage('Test') {
            steps {
                echo 'Mengecek file index.html...'
                sh 'ls -l public/index.html'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Menyalin file ke Nginx...'
                sh 'cp -f public/index.html /var/www/html/index.html'
            }
        }
    }
}
