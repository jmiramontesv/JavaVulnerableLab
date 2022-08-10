pipeline {
    agent any
    tools {
        maven "Maven-3.8.5"
        jdk "OpenJDK11"
    }
    stages {
        stage('Initialize'){
            steps{
                echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /opt/maven"
            }
        }
        stage('Build') {
            steps {
                dir("/var/lib/jenkins/workspace/JavaVuln_Pipeline/JavaVulnerableLab") {
                sh 'mvn -B -DskipTests clean package'
                }
            }
        }
     }
    
}
