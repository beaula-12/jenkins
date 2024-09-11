pipeline {
    agent any

    stages {
        stage('GitHub Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/beaula-12/jenkins.git'
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
