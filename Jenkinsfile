pipeline {
  agent any
  stages {
    stage('Tasks') {
      steps {
        parallel(
          "Tasks": {
            tool(name: 'Gradle 3.5', type: 'gradle')
            
          },
          "Tasks2": {
            sh 'gradle tasks'
            
          },
          "Tasks3": {
            sh 'gradle tasks'
            
          }
        )
      }
    }
    stage('Components') {
      steps {
        tool(name: 'Gradle 3.5', type: 'gradle')
        sh 'gradle components'
      }
    }
    stage('Test') {
      steps {
        tool(name: 'Gradle 3.5', type: 'gradle')
        sh 'gradle test'
      }
    }
  }
}