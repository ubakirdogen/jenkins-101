pipeline {
    agent { 
        node {
            label 'docker_agent_alpine_py'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh '''
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python helloworld.py
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
