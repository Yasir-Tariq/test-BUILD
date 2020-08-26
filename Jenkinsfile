pipeline {
    agent any
    parameters {
          string(defaultValue: 'RDBJOB', description: 'Enter version', name: 'VERSION')
    }
    stages {
        stage ('BRANCH'){
            steps {
                sh "echo ${env.BRANCH_NAME}"
            }
        }
        stage ('Build'){
            steps {
                sh "echo ${params.VERSION}"
            }
        }
    }
} 
