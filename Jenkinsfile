pipeline{
                stages{
		        agent {
                                label "slave1"
                              }

                        stage ("Pull the code latest from SCM"){

                               steps {
                                        git branch: 'main', url: 'https://github.com/devsharma1401/project-1.git'
                                        }
                                }
		        agent {
                                 label "slave-2"
                              }

                        stage (" Build the code "){

                                steps {
                                        sh 'sudo mvn clean package'
                                        }
                                }
                }
        }


