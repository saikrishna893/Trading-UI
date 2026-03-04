pipeline {
    agent any

    tools {
        nodejs "Node-16"
    }

    stages {
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
               sh 'CI=false npm run build'
            }
        }
    }
}
