pipeline {
    agent none
    options {
        disableConcurrentBuilds()
    }
    stages {

        stage('First stage') {
            agent any
            steps {
                sshagent(credentials: ['github']) {
                    sh 'ssh -T git@github.com || exit 0'
                }
                sleep 10000
            }
        }

    }
}
