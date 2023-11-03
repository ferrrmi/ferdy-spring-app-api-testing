pipeline {
    agent {
        node {
            label "linux && java11 && java17"
        }
    }
    stages {
        stage('Build') {
            steps {
                echo 'hello Build!'
            }
        }

        stage('Test') {
            steps {
                echo 'hello test!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'hello deploy!'
            }
        }
    }
    post {
        always {
            echo "i will always says hello again"
        }
        success {
            echo 'i will return this if the pipeline is success'
        }
        failure {
            echo 'i will return this if the pipeline is error / fail'
        }
        cleanup {
            echo 'this will cleanup, dont care if the pipeline is error / success'
        }
    }
}