pipeline {
    agent any
    stages {
      stage('Build') {
          steps {
            echo 'Build running'
            sh './gradlew build --no-daemon'
            archiveArtifacts artifacts: 'dist/trainSchedule.zip'
          }
      }
    }
}
