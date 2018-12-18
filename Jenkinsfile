pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'build'])
        archiveArtifacts(artifacts: '*.sh', fingerprint: true)
      }
    }
  }
}