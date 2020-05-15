pipeline {

  agent any
  
  stages {
    
    stage ('Build') {
      steps {
        echo 'Running Build Automation Step'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
