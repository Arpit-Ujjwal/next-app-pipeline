pipeline {
    agent any
    tools {nodejs "nodejs"}
    stages {
        stage("checkout") {
            steps {
                checkout scm
            }
        }

        stage("install") {
            steps {
                sh 'npm i'
            }
        }

        stage("Build") {
            steps {
                sh 'npm run build'
            }
        }
    }
}