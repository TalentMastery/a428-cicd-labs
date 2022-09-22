node {
    stage('docker') {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
    stage('built') {
        sh 'npm install' 
    }
    stage('test') {
        sh './jenkins/scripts/test.sh'
    }
}