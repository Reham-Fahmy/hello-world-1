pipeline {
    agent any
    parameters {
        choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: '')
        booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
    stages {
        stage("init") {
            steps {
                echo'build init stage' 
                }
            }
        }
        stage("build") {
            steps {
                echo'build2 stage'
                }
            }
        }
        stage("test") {
            when {
                expression {
                    params.executeTests
                }
            }
            steps {
                echo'build test stage'
                }
            }
 
        stage("deploy") {
            steps {
                echo'build deploy stage'
                }
            }
      
    }   
}
