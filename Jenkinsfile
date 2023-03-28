pipeline {
    agent any
    environment {
        p = sh 'echo $PATH'
        PATH = p + ':/usr/local/bin/docker-compose'
    }
    stages {
        stage('build') {
            steps {
                echo "Hello World"
                sh 'echo using shell within Jenkinsfile'
                echo 'not using shell in the Jenkinsfile'
                sh 'cat ./example.txt'
                sh 'pwd'
                sh "cd /var/lib/jenkins/workspace/github-hook"
                sh '/usr/local/bin/docker-compose down'
                sh '/usr/local/bin/docker-compose up -d --build'
                echo 'it works111'                
            }
        }
    }
}
