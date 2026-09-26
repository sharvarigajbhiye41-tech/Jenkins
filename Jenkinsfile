pipeline {
    agent any
    stages {
    stages('Build){
           steps { sh 'echo Building' } 
        }
        stage('Tests') {
            parallel {
                stage('Unit') {steps { sh 'echo Unit tests }  }
                stage('Integration') {steps { sh 'echo Integration tests'}}
            }
        }
    }
}
