pipeline {
    agent any
    stages {
    stage ("Master") {
            when {
                branch 'master'
            }
            steps { 
                echo "master"
            }            
        }
        stage ("Main") {
            when {
                branch 'main'
            }
            steps {
                echo "Nohing will come"
            }
        }
    }
}
