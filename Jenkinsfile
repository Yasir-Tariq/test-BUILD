pipeline {
    agent any
    parameters {
          string(description: 'Enter version', name: 'VERSION')
    }
    stages {
        stage ('Build'){
            steps {
                script {
                    if ("${params.VERSION}".isEmpty()) {
                        error('Version is not provided!')
                    }
                    else {
                        sh "echo Building using Version: ${params.VERSION}"
                    }
                }
                
            }
        }
        stage ('Publish') {
            steps {
                script {
                    sh "echo Publishing using Version: ${params.VERSION}"
                }
            }
        }
    }
} 
