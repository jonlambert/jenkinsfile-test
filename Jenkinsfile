pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'New script...'
            }
        }
        stage('Test') {
                steps {
                echo 'Testing..'
		        echo 'This works well'
            }
        }
        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo 'Deploying....'
                sh 'rsync --exclude ".git" -avz . ~/var/www/toshi'       
            }
        }
    }
}
