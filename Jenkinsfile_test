pipeline {
            agent any
            stages {
                      stage ('maven build') {
                                  steps {
                                              sh 'mvn test package'
                                              }
                                   post{
                                              archiveArtifacts artifacts : '**/*.war'
                                               }
                                               }
                     }
           }
