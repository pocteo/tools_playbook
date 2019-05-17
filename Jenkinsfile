node('ansible-kubectl') {
  stage('deploy tools') {
    sh 'ansible-galaxy install -r requirements.yml --roles-path ./roles'
    sh 'ansible-playbook playbook.yml'
  }
}
