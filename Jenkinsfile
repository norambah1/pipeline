Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                sh 'mvn --v'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
