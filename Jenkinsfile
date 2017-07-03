pipeline {
  agent any
  stages {
    stage('Tasks') {
      steps {
        tool(name: 'Gradle 3.5', type: 'gradle')
        sh 'gradle tasks'
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