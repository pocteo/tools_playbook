node('ci-docker-slave') {
  stage('docker push') {
    sh 'docker version'
    git(url: 'https://github.com/pocteo/boilerplate-node-api.git', branch: 'master')
    sh 'docker login -u pocteo -p @hi_pocteo'
    sh 'docker build -t pocteo/nodejs_app:pr-6 .'
    sh 'docker push pocteo/nodejs_app:pr-6'
  }
}
