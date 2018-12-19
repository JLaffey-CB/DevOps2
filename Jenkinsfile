pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'build/master'])
        archiveArtifacts(artifacts: '*.sh', fingerprint: true)
      }
    }
  }
}
