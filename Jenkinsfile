def lv
pipeline {
    agent any

    stages {
        
        stage{
            script{
                gv = load "script.groovy"
            }
        }
        
        stage ('Checking ') {
            scripts {
                lv.buildApp()
            }
        }
    }
}
