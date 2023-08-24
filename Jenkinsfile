node {
  git branch: 'main', url: 'https://github.com/SiwatINC/node-baseimage'
  docker.withRegistry("https://ghcr.io/v2") {
      docker.build("siwatinc/node-baseimage:node12",'node12').push()
      docker.build("siwatinc/node-baseimage:node16",'node16').push()
      docker.build("siwatinc/node-baseimage:node18",'node18').push()
  }
}
