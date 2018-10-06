pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running Build"
        sh './gradlepw build --no-daemon'
        archiveArifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
