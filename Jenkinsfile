pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('build') {
            steps {
                sh 'node --version'
                nodejs(node-10.17){
                    sh'yarn install'}
            }
        }
    }
}
