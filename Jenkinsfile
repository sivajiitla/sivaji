pipeline {
            agents any
            stages {
                      stage ('maven build') {
                                              sh ('mvn test package')
                                              }
                      stage('archive artifact'){
                                              archiveartifact artifact: * */*war
                                               }
                     }
           }
