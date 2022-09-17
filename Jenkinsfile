def lv
pipeline {
    agent any
    script{
        gv = load "script.groovy"
    }
    stages {
        stage ('Checking ') {
            scripts {
                lv.buildApp()
            }
        }
    }
}
