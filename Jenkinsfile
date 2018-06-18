pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'test-1/master'])
        step([$class: 'CopyArtifact', projectName: 'test-2/master'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
        echo 'deploy successful'
      }
    }
  }
}
