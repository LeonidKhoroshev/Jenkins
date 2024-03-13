pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Clear work dir') {
            steps {
                deleteDir()
            }
        }
        stage('Clone git repo') {
            steps {
                dir('vector-role') {
                git branch: 'molecule', url: 'https://github.com/LeonidKhoroshev/vector.git'
                }
            }
        }
    }
