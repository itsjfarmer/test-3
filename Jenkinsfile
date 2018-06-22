pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
        //step([$class: 'CopyArtifact', projectName: 'test-1/master'])
        //step([$class: 'CopyArtifact', projectName: 'test-2/master'])
        //archiveArtifacts artifacts: '*.sh', fingerprint: true
	devOpticsConsumes jobName: 'test-1/master'
	devOpticsConsumes jobName: 'test-2/master'
        echo 'deploy successful'
      }
    }
  }
}
