pipeline {
      agent {label "slave-3"}
        stages {
               stage('Welcome') {
                                steps {
                                     sh '''
                                            pwd
                                            sleep 5
                                            echo "welcome"
                                     '''
                                }
                }
                stage ('create_directory') {
                                   steps {
                                         sh '''
                                             mkdir test_pipeline
                                         '''
                                    }
                 }
                stage ('create_File') {
                                  steps {
                                       sh '''
                                           touch jenkisfile
                                       '''
                                  }
                }
                                  
                
        }
}
