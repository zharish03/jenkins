def lv
pipeline {
    agent any

    stages {
        
        stage ('Scripts') {
            steps{    
                script{
                    lv = load "scripts.groovy"
                }
            }    
        }
        
        stage ('Building') {
            steps{
                scripts {
                    lv.buildApp()
                }
            }
        }
    }
}


