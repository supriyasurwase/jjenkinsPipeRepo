pipeline {
    agent any
    stages {
	// clone the repository
        stage('Clone Repository') {
            steps {
              git branch: 'main'  , url: 'https://github.com/supriyasurwase/jjenkinsPipeRepo.git'  // Replace with your repo URL
            }
        }
	// Deploy the index.html file
        stage('Deploy HTML file') {
            steps {
		sh '''
		# Deploy index.html file to the web server directory
		cp index.html /var/www/html/
		'''
            }
        }
    }
}