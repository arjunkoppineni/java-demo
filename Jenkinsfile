pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Jenkins automatically checks out the repo with 'checkout scm'
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling Hello.java...'
                sh 'javac Hello.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Hello.java...'
                sh 'java Hello'
            }
        }
    }
}
