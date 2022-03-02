// Jenkinsfile (Declarative Pipeline)

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                export JAVA_HOME="/Library/Java/JavaVirtualMachines/jdk1.8.0_311.jdk"
                export MAVEN_HOME="/usr/local/Cellar/maven/3.8.4/libexec"
                export PATH="$PATH:$MAVEN_HOME/bin"
                mvn -version
                echo "building"
                mvn compile
                '''
            }
        }
    }
}
