pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '''-p 3000:3000
-e "http_proxy=http://PITC-Zscaler-AmericasZ.proxy.corporate.ge.com:80"
-e "https_proxy=http://PITC-Zscaler-AmericasZ.proxy.corporate.ge.com:80"'''
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}