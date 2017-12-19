node {
    checkout scm
    docker.withRegistry('http://192.168.99.102:5000/v2/') {
        def customImage = docker.build("my-nginx:${env.BUILD_ID}")
        customImage.push()
    }
}
