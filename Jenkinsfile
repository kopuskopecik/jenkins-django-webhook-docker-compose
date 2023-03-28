```groovy
pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                echo "Hello World"
                sh 'echo using shell within Jenkinsfile'
                echo 'not using shell in the Jenkinsfile'
            }
        }
    }
}
```
