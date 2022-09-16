pipeline {

    agent any
    stages{
        
        stage ('Build') {
            steps {

                cleanWs()
                sh 'echo "harish" > text.txt'
                sh 'mkdir harish tex'
            
            }
        }        
        
        stage ('ENV-Testing') {
            steps {
                echo 'This is ${BRANCH_NAME}'
            }
        }
    }
}
