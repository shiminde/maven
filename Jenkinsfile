pipeline {
  agent any
  stages {
    stage('start') {
      agent any
      steps {
        echo 'Start'
      }
    }
    stage('build') {
      agent any
      steps {
        sh 'mvn clean package'
      }
    }
    stage('') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }
  }
}