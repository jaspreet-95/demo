pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('test') {
      steps {
        sh '''test "comiple"
'''
      }
    }

    stage('package') {
      steps {
        sh 'mvn package'
      }
    }

    stage('archeive the ') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }

    stage('publish result') {
      steps {
        junit '**/*xml'
      }
    }

  }
}