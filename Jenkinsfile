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
                      sh 'make build'
                      sh 'pwd'
                      sh 'ls -lrt'
                      //sh './node_modules/grunt-cli/bin/grunt test'
                      sh 'hack/verify-dist.sh'
                    } // steps
                } // stage
            } // stages
        } // pipeline
