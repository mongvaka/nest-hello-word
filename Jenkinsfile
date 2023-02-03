pipeline{
    agent any
    tools {
        maven "M3"
    }
    stages {

        stage ("Complie")
        steps {
            sh "mvn clean complie"
        }
        stage ("Test") {
            steps {
                sh "mvn clean test"
            }
        }
        stage ('Deploy') {
            sh "mvn clean install"
        }
    }
}