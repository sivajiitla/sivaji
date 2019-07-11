pipeline {
            agent any
            stages {
                      step ('maven build') {
                                              sh ('mvn test package')
                                              }
                      post('archive artifact'){
                                              archiveArtifacts artifacts : '**/*.war'
                                               }
                     }
           }
