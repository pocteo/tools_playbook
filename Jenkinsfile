node('ansible-kubectl') {
  stage('deploy tools') {
    git(url: 'https://github.com/pocteo/tools_playbook.git', branch: 'master')
    sh 'ansible-galaxy install -r requirements.yml --roles-path ./roles'
    sh 'ansible-playbook playbook.yml'
  }
}
