node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'dockerhub-suusar') {

        def customImage = docker.build("suusardzh/node.js-app}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
