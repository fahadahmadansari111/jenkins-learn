pipeline {
    agent any
    environment {
        mavenHome = tool 'myMaven'
        dockerHome = tool 'myDocker'
        PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                sh 'docker version'
            }
        }
    }
}