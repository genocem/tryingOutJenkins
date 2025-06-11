pipeline {
	agent any
    stages {
        stage('build') {
            steps {
            	echo "beninging"
            	sshagent(credentials: ['SSH_PRIVATE_KEY']) {
                sh ''' 
		        ssh -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ubuntu@10.71.165.172 '
		        echo "hello" > hewwo
                '   
                '''
}
                
            }
        }
    }
}
