pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/yourusername/your-repo.git'
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh '''
                    sudo cp -r * /var/www/html/
                    '''
                }
            }
        }
    }
}
