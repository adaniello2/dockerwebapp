node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'duckerHub') {

        def customImage = docker.build("adani/dockerwebapp}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}