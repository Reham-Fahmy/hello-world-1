pipeline {
    agent any
    parameters {
        choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: '')
        booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
}
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
