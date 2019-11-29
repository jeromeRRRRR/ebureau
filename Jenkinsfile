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
				bat 'mvn clean test'
            }
        }
        stage('Packaging') { 
            steps {
                // 
				echo 'Etape Packaging'
				bat 'mvn clean package'
            }
        }
		stage('Deploy') { 
            steps {
                // 
				echo 'Etape Deploy'
				copy /Y "C:\opt\Jenkins\workspace\ebureauPipeline\target\ebureau.war" "C:\Program Files\Apache Software Foundation\Tomcat 9.0\webapps\ebureau.war"
            }
        }
    }
}