pipeline {
    agent {
        node{
            label 'maven-agent'
        }
    }
environment {
    PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
}
    stages{
        stage('Clone code') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}