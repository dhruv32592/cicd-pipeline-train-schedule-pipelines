pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
      }
    }
    stage ('Archive'){
      steps{
        echo 'Archiving your awesome artifact'
        archiveArtifacts artifacts: dist/trainSchedule.zip      
      }
    }
  }
}
