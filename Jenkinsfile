// Jenkinsfile (Declarative Pipeline)

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                echo $M2_HOME
                PATH=$PATH:$M2_HOME/bin
                java -version
                mvn -version
                echo "building"
                mvn compile
                '''
            }
        }
    }
}
