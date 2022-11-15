pipeline {
    agent any

    stages {
        stage('test parallel'){
        parallel{
        stage('build') {
            steps {
                echo 'Hello World - from git test'
                git branch: 'main', url: 'https://github.com/johnchellaiayan/jenkintest.git'
            }
        }
         stage('run') {
            steps {
                echo ' Run Hello World'
            }
        }
        }
        }
    }
}
