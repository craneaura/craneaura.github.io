pipeline {
  agent any
  stages {
    stage('pull') {
      parallel {
        stage('pull') {
          steps {
            timestamps() {
              git(url: 'https://github.com/craneaura/craneaura.github.io.git', branch: 'master', changelog: true)
            }

          }
        }

        stage('Sleep') {
          steps {
            sleep 3
          }
        }

      }
    }

    stage('Print') {
      steps {
        echo 'Hello World'
      }
    }

  }
}