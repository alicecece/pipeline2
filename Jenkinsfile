pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('ooh') {
          steps {
            sh 'echo hello world'
          }
        }
        stage('aah') {
          steps {
            mail(subject: 'jenkins test', body: 'this is a jenkins test', from: 'jenkins', to: 'wualice017@gmail.com')
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