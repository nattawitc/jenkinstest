pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('build') {
            steps {
                sh 'go build -o bin'
                sh './bin'
            }
        }
        stage('test') {
            steps {
                sh 'go test'
            }
        }
    }
}
