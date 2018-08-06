        pipeline {
            agent {
              node {
                label 'nodejs'
              }
            }
            options {
                timeout(time: 20, unit: 'MINUTES')
            }
            stages {                                
                stage('build') {
                    steps {
                      sh 'ls -lrt'
                    } // steps
                } // stage
            } // stages
        } // pipeline
