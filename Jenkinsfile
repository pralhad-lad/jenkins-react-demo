pipeline {
    agent any

    stages {
        stage ('CLone') {
            steps {
                git 'https://github.com/pralhad-lad/jenkins-react-demo.git'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Success') {
            steps {
                echo 'React App Build  completed'
            }
        }
    }
}