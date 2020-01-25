pipeline {
    agent any 
    stages {
        stage('deployement') { 
            steps {
            sh '''
       	          #!/bin/bash
                   set -x
                   echo "apache installation in progress"
                   cd ${WORKSPACE}
                   ansible-playbook -u root -l integration ansible.yml
                    set +x
	        ''' 
            }
        }
        
      }
    }
