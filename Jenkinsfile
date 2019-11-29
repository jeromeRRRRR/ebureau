pipeline {
    agent any

	tools {
		maven 'M3'
	}
	
    stages {
	
        stage('Compile') { 
            steps {
                // 
				echo 'Etape compile'
				bat 'mvn clean compile'
            }
        }
        stage('Test') { 
            steps {
                //
				echo 'Etape compile'
            }
        }
        stage('Packaging') { 
            steps {
                // 
				echo 'Etape Packaging'
            }
        }
		stage('Deploy') { 
            steps {
                // 
				echo 'Etape Deploy'
            }
        }
    }
}