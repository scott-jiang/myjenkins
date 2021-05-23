pipeline {
  agent any
  stages {
    stage('Windows Host Step') {
        steps{
          dir(path: 'ansible') {
            ansiColor(colorMapName: 'xterm') {
              ansiblePlaybook(
                playbook: 'playbook.yml',
                inventory: 'inventory',
                colorized: true)
            }
          }
        }
    }
  }
}
