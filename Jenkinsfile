pipeline {
    agent any

    stages {
        stage('Compile stage') {
            steps {
                withMaven(maven : 'M2_HOME) {
                  sh 'mvn clean compile'
                  }
            }
        }
        stage('Testing stage') {
            steps {
                withMaven(maven : 'M2_HOME) {
                  sh 'mvn test'
                  }
            }
        }
        stage('Deploy stage') {
            steps {
                withMaven(maven : 'M2_HOME) {
                  sh 'mvn install'
                  }
            }
        }
    }
}
