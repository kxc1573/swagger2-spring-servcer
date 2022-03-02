// Jenkinsfile (Declarative Pipeline)

export MAVEN_HOME=/usr/local/Cellar/maven/3.8.4/libexec
export PATH=$PATH:$MAVEN_HOME/bin

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                mvn -version
                echo "building"
                mvn compilem
                '''
            }
        }
    }
}
