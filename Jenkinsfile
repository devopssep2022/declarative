pipeline {
      agent none
        stages {
              agent {label "slave-2"}
               stage('Welcome') {
                                steps {
                                     sh '''
                                            pwd
                                            sleep 5
                                            echo "welcome"
                                     '''
                                }
                }
              agent {label "slave-3"}
              stage ('create_directory') {
                                   steps {
                                         sh '''
                                             mkdir test_pipeline
                                         '''
                                    }
                 }
              agent { label "slave-2"}
                stage ('create_File') {
                                  steps {
                                       sh '''
                                           touch jenkisfile
                                       '''
                                  }
                }
                                  
                
        }
}
