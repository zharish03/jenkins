def gv
pipeline {
    agent any

    stages {
        
        stage("init") {
            steps {
                script {
                   gv = load "script.groovy" 
                }
            }
        }

        stage ("Building") {
            steps {
                scripts {
                    gv.buildApp()
                }
            }
        }
    }
}

