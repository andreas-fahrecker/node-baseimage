node {
  git branch: 'main', url: 'https://github.com/SiwatINC/node-baseimage'
  docker.withRegistry("https://ghcr.io/v2") {
      docker.build("siwatinc/python-baseimage:node12",'node12').push()
      docker.build("siwatinc/python-baseimage:node16",'node16').push()
  }
}
