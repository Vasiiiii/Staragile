pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('Deploy') {
            steps {
                // Add deployment steps here
                // For example, deploying to Tomcat
                sh 'sudo cp target/your-application.war /var/lib/tomcat9/webapps/'
            }
        }
        
        // Add more stages as needed
    }
}
