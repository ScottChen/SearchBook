pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'test test test'
      }
    }

    stage('stage2') {
      steps {
        timestamps() {
          writeFile(file: 'hello', text: 'hello world', encoding: 'utf-8')
        }

      }
    }

    stage('stage3') {
      steps {
        sh 'echo "hello, world"'
      }
    }

  }
}