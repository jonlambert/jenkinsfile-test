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
            steps {
                echo 'Deploying....'
                rsync -avz . /deployment-test-folder
            }
        }
    }
}
