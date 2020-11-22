node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("docker_web_app/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}