def lv
pipeline {
    agent any
    parameters {
        booleanParam(name: 'executeTests', defaultValue: true, description:'')
        )
    }
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
        stage ("When Condition") {
            when {
                params.executeTests
            }
            steps {
                script {
                    lv.testApp()
                }
            }
        }
    }
}
