node('docker') {
  stage('docker push') {
    git(url: 'https://github.com/pocteo/nodejs_app.git', branch: 'master')
    sh 'docker login -u pocteo -p @hi_pocteo'
    sh 'docker build -t pocteo/nodejs_app:pr-6'
    sh 'docker push pocteo/nodejs_app:pr-6'
  }
}
