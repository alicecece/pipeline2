pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo hello world'
          }
        }
        stage('error') {
          steps {
            emailext(subject: 'test', body: 'jenkins test', from: 'jenkins', to: 'wualice017@gmail.com')
          }
        }
      }
    }
    stage('stage2') {
      steps {
        echo 'this is from stage 2'
      }
    }
  }
}