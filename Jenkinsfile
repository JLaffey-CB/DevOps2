pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'application-build'])
        archiveArtifacts(artifacts: '*.sh', fingerprint: true)
      }
    }
  }
}