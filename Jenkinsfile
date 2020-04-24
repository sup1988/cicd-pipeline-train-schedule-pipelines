pipeline {
  agent any
    stages {
      stage ('Build') {
        steps {
          echo 'Running Automated Build'
          sh './gradlew build --no-daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        }
      }
  }
}
