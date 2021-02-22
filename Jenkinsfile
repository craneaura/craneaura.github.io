pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        git(url: 'https://github.com/craneaura/craneaura.github.io.git', branch: 'master', changelog: true)
      }
    }

    stage('Print') {
      steps {
        echo 'Hello World'
      }
    }

  }
}