pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'test-1'])
        step([$class: 'CopyArtifact', projectName: 'test-2'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
        echo 'deploy successful'
      }
    }
  }
}
