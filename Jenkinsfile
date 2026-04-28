pipeline {
    agent none

    stages {

        stage('Run on VM1') {
            agent { label 'rudra-vm1' }
            steps {
                sh 'python3 hello.py'
            }
        }

        stage('Run on VM2') {
            agent { label 'rudra-vm2' }
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
