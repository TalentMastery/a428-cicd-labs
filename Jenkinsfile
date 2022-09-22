node {
    stage('built'){
        withDockerContainer(image: 'node:lts-bullseye-slim', args: '-p 3000:3000' )
        sh 'npm install' 
    }
    stage('test'){
        sh './jenkins/scripts/test.sh'
    }
}
