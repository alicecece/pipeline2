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
        stage('') {
          steps {
            mail(subject: 'jenkins test', body: 'this is a test', to: 'wualice017@gmail.com', from: 'jenkins')
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