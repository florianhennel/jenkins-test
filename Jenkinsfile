pipeline {
    agent { 
        node {
            label 'docker-agent-alpine'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo 'doing build stuff..'
                echo 'and building more..'
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo 'doing testing stuff..'
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