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
                    else if (params.VERSION.contains('dev')) {
                        //sh "make build TAG=${VERSION.substring(8)}"
                        sh "echo Building using Version: ${VERSION.substring(8)}"
                    }
                    else {
                        //sh "make build TAG=${VERSION.substring(9)}"
                        sh "echo Building using Version: ${VERSION.substring(9)}"
                    }
                }
                
            }
        }
        stage ('Publish') {
            steps {
                script {
                    if (params.VERSION.contains('dev')) {
                        //sh "make publish TAG=${VERSION.substring(8)}"
                        sh "echo Publishing using Version: ${VERSION.substring(8)}"
                    }
                    else {
                        //sh "make publish TAG=${VERSION.substring(9)}"
                        sh "echo Publishing using Version: ${VERSION.substring(9)}"
                    }
                }
            }
        }
    //    stage('ONE') {
      //      steps {
        //        catchError {
          //          sh "echo this is first stage"
            //        sh "make abc"
              //  }
                //echo currentBuild.result
           // }
        //}
        //stage('TWO') {
          //  steps {
            //    sh "echo this is second stage"
            //}
        
        
        
        
        
      
    }
} 
