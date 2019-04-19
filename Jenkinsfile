node {
    checkout scm

    docker.withRegistry('https://cloud.docker.com/u/adaniello1/repository/docker/adaniello1/mydockerhub', 'dockerHub') {

        def customImage = docker.build("adani/dockerwebapp}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
