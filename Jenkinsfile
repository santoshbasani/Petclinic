pipeline {
    agent any
    
    tools {
        jdk 'jdk11'
        maven 'maven'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'featre-1', url: 'https://github.com/jaiswaladi246/Petclinic.git'
            }
        }
        
        stage('Compile') {
            steps {
                sh "mvn clean package"
            }
        }
        
    }
}
