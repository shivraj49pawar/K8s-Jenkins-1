pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        writeFile(file: 'Hello.txt', text: 'Hi WP')
      }
    }

    stage('Read YAML') {
      steps {
        readFile 'pods.yml'
      }
    }

  }
}