pipeline {
    agent {
        node {
            label "linux && java11 && java17"
        }
    }
    stages {
        stage('hello') {
            steps {
                echo 'hello world!'
            }
        }
    }
}