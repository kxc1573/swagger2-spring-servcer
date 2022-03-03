// Jenkinsfile (Declarative Pipeline)

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                java -version
                mvn -version
                echo "building"
                mvn compile
                '''
            }
        }
    }
}
