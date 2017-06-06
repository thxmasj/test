pipeline {
    agent none
    options {
        disableConcurrentBuilds()
    }
    stages {

        stage('First stage') {
            agent any
            steps {
                sh 'ssh -T git@github.com'
                sleep 10000
            }
        }

    }
}
