node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'dockerHub') {

        def customImage = docker.build("nodejs/web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}