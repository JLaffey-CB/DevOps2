pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'cray/Build/master'])
        archiveArtifacts(artifacts: '*.sh', fingerprint: true)
      }
    }
  }
}
