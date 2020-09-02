pipeline {
    agent any
    //parameters {
    //      string(description: 'Enter version', name: 'VERSION')
    //}
    stages {
        stage('ONE') {
            steps {
                catchError {
                    sh "echo this is first stage"
                    sh "make abc"
                }
                echo currentBuild.result
            }
        }
        stage('TWO') {
            steps {
                sh "echo this is second stage"
            }
        }
        
        
        
        
        
        
        
        
        
        //stage ('Build'){
           // steps {
              //  script {
               //     if ("${params.VERSION}".isEmpty()) {
               //         error('Version is not provided!')
               //     }
                //    else {
                //        sh "echo Building using Version: ${params.VERSION}"
                 //   }
                //}
                
            //}
       // }
       // stage ('Publish') {
        //    steps {
          //      script {
          //          sh "echo Publishing using Version: ${params.VERSION}"
           //     }
           // }
       // }
    }
} 
