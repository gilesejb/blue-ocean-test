pipeline {
  agent any
  stages {
    stage('Tasks') {
      steps {
        parallel(
          "Tasks": {
            sh 'gradle tasks'
            
          },
          "Components": {
            sh 'gradle components'
            
          },
          "Test": {
            sh 'gradle test'
            
          }
        )
      }
    }
  }
}