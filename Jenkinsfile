pipeline {
    
    agent any

    stages {

        stage('Checkout') {

            steps {
                checkout scmGit(branches: [[name: '*/main'], [name: '*/b1']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/tomanstensen/Jenkinslab.git']])
            }
        }

        stage('Build') {
            steps {
                echo 'build me'
            }
        }
        stage('Test') {
            steps {
                echo 'testy'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy?'
            }
        }

         stage('Run Robotframe') {
            steps {
                echo 'run robot'
            }
        }

         stage('Post RobotTests') {
            steps {
                echo 'post robot'
            }
        }
    }
}