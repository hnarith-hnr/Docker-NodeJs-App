node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'hnarith') {

        def customImage = docker.build("nodejs/web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
