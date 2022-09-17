def gv

pipeline {
    agent any

    stages {
        stage("init") {
            steps {
                script {
                   gv = load "scripts.groovy" 
                }
            }
        }
        stage("build") {
            steps {
                script {
                    gv.buildApp()
                }
            }
        }
        stage("deploy") {
            steps {
                script {
                    gv.deployApp()
                }
            }
        }
    }   
}

