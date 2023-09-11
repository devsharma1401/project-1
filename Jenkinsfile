pipeline{
                stages{
                        stage ("Pull the code latest from SCM"){
                               agent {
                                       label "slave1"
                                     }

                               steps {
                                        git branch: 'main', url: 'https://github.com/devsharma1401/project-1.git'
                                        }
                                }
                        stage (" Build the code "){
                                agent {
                                       label "slave-2"
                                     }

                                steps {
                                        sh 'sudo mvn clean package'
                                        }
                                }
                }
        }


