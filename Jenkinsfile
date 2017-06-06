pipeline {
    agent none
    options {
        disableConcurrentBuilds()
    }
    stages {

        stage('First stage') {
            agent any
            steps {
                sleep 10000
                sh 'ssh -T git@github.com'
            }
        }

    }
}
