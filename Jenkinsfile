pipeline {
    agent any

    stages {
        stage('Presetup') {
            steps {
                echo 'Preparing the environment..'
            }
        }
        stage('DEV Step') {
            steps {
                echo 'Executing DEV Script..'
                sh '' sh dev.sh ''
            }
        }
        stage('SIT Step') {
            steps {
                echo 'Executing SIT Script..'
                sh '' sh sit.sh ''
            }
        }
        stage('UAT Step') {
            steps {
                echo 'Executing UAT Script..'
                sh '' sh uat.sh ''
            }
        }
        stage('Clean') {
            steps {
                echo 'Destroying..'
            }
        }
    }
}
