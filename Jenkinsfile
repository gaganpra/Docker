node {

    checkout scm

   docker.withRegistry('https://registry.hub.docker.com', 'Docker_Build') {

        def customImage = docker.build("gaganpr/myimage1")

        /* Push the container to the custom Registry */

        customImage.push()

    }

}
