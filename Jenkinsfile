pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'test-3'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
        echo 'deploy successful'
      }
    }
  }
}
