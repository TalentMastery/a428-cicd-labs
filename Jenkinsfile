node {
    docker.image('node:lts-buster-slim').inside('-p 3000:3000'){
        withEnv(['CI=true']){
            stage('built'){
                sh 'npm install'
            }
            stage('test'){
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}