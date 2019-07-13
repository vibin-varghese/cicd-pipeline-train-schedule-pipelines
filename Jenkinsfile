pipeline {
  agent any {
    stages {
      stage('Build') {
        echo 'Build running'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
