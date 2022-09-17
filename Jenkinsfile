def lv
pipeline {
    agent any
    stages {
        stage ('Checking') {
            steps {
                script {
                    lv = load "scripts.groovy"
                }
            }
        }
        stage ('Building') {
            steps {
                script {
                    lv.buildApp()
                }
            }
        }
    }
}
