pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/beaula-12/jenkins'
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
