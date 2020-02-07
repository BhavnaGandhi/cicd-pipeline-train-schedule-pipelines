pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
