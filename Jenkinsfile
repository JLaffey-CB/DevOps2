pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'Build'])
        archiveArtifacts(artifacts: '*.sh', fingerprint: true)
      }
    }
  }
}