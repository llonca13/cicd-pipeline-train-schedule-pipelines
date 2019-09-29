pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running build automations"
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
