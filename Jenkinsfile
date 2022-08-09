pipeline {
    agent any
    tools {
        jdk 'AdoptOpenJDK11'
        maven 'Maven_3_8_1'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
