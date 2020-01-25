pipeline {
    agent any 
    stages {
        stage('deployement') { 
            steps {
            sh '''
       	          #!/bin/bash
                   set -x
                   cd ${WORKSPACE}
                   ansible-playbook -u root -l integration ansible.yml
                    set +x
	        '''
		// 
            }
        }
        
            }
        }
