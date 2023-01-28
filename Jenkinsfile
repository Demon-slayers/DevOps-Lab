pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Post') {
            steps {
                echo 'Posting....'
            }
        }
    }
}

post{
  always{
    emailext body: 'Summary', replyTo: 'shonitaric@gmail.com', subject: 'Jenkins Pipeline', to: 'shonitaric@gmail.com'
  }
}

