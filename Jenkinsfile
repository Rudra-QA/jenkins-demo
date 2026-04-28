pipeline {
    agent none

    stages {

        stage('Run app on VM1') {
            agent { label 'rudra-vm1' }
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Run app on VM2') {
            agent { label 'rudra-vm2' }
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
