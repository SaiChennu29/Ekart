pipeline {
    agent any
    
    tools { maven 'maven3.6'
            jdk 'jdk11'
    }
    stages {
        stage('git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/SaiChennu29/Ekart.git'
            }
        }
         stage('compile') {
            steps {
               sh "mvn compile"
            }
        }
    }
}
