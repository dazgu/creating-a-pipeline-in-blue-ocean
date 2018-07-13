pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
  environment {
    http_proxy = 'http://PITC-Zscaler-AmericasZ.proxy.corporate.ge.com:80'
    https_proxy = 'http://PITC-Zscaler-AmericasZ.proxy.corporate.ge.com:80'
  }
}