pipeline {
    agent { 
        docker {
            image 'docker:dind'
            args '-v /var/run/docker.sock:/var/run/docker.sock -e HOME=${workspace}'
        }
    }
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
