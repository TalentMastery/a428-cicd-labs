node {
    stage('built'){
        withDockerContainer(image: 'node:lts-bullseye-slim', args: '-p 3000:3000')
    }
}