pipeline {
    agent { docker { image 'docker:dind' } }
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
