pipeline {
    agent any
    tools {
        maven "Maven-3.8.5"
        jdk "OpenJDK11"
    }
    stages {
       stage('Build') {
            steps {
                dir("C:\\Jenkins_Workspace\\workspace\\JavaVuln_Pipeline\\JavaVulnerableLab") {
                sh 'mvn -B -DskipTests clean package'
                }
            }
        }
     }
    
}
