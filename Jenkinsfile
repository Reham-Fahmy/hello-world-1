pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('test') {
            steps {
                sh 'node --version'
                withGradle(Gradle)
                sh'./gradlew -v'
                
            }
        }
    }
}
