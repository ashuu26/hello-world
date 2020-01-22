pipeline {
    agent any

    stages {
        stage('Compile stage') {
            steps {
                withMaven(maven : '') {
                  sh 'mvn clean compile'
                  }
            }
        }
        stage('Testing stage') {
            steps {
                withMaven(maven : '') {
                  sh 'mvn test'
                  }
            }
        }
        stage('Deploy stage') {
            steps {
                withMaven(maven : '') {
                  sh 'mvn install'
                  }
            }
        }
    }
}
