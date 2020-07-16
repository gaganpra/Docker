node {

    checkout scm

   docker.withRegistry('https://registry.hub.docker.com', 'docker-build') {

        def customImage = docker.build("gaganpra/myimage1")

        /* Push the container to the custom Registry */

        customImage.push()

    }

}
