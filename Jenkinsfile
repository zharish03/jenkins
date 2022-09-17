def lv
pipeline {
    agent any

    stages {
        
        stage ('Scripts'){
            script{
                gv = load "script.groovy"
            }
        }
        
        stage ('Building') {
            scripts {
                lv.buildApp()
            }
        }
    }
}
