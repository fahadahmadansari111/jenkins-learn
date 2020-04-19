pipeline {
    agents any
    mavenHome = tool 'myMaven'
    dockerHome = tool 'myDocker'
    PATH = "$dockerHome/bin:$mavenHone/bin:$PATH"
}

stages {
    stage('Build') {
        steps {
            sh 'mvn --version'
            sh 'docker version'
        }
    }
}