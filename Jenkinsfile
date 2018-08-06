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
                      sh 'alias grunt=/tmp/workspace/run9io-dev/run9io-dev-origin-web-console/node_modules/grunt-cli/bin/grunt'
                      sh 'hack/verify-dist.sh'
                    } // steps
                } // stage
            } // stages
        } // pipeline
