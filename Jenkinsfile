// Powered by Infostretch 

timestamps {

node () {

	stage ('ansible-pre-prod - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/release']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '80f3a06e-c792-4eee-a408-57ebaa0aee8f', url: 'https://github.com/Salmaa182/finalproject.git']]]) 
	}
	stage ('ansible-pre-prod - Build') {
 			// Shell build step
sh """ 
#!/bin/bash

set -x

cd ${WORKSPACE}

ansible-playbook -u root -l preprod ansible.yml

set +x 
 """ 
	}
}
}