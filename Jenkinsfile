pipeline {
    agent { dockerfile true }
    stages {
        stage('build') {
            steps {
                script {
                    docker.build("my-app:latest")
                }
            }
        }
    }
}
