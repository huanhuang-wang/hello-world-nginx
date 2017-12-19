node {
    checkout scm
    docker.withRegistry('http://192.168.99.101:5000/v2/') {
        def customImage = docker.build("invast.jp/mh/my-nginx:${env.BUILD_ID}")
        customImage.push()
    }
}
