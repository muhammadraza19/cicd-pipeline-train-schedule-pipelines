pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifactcs: 'dist/trainSchedule.zip'
      }
    }
  }
}
