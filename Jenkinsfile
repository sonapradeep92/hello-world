pipeline {
    agent any
    environment {
        PATH="/opt/apache-maven-3.9.0/bin:$path"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('SCM') {
            steps {
                git 'https://github.com/sonapradeep92/hello-world.git'
            }
        }
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
