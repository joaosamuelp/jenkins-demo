pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        writeFile(file: 'teste-file.txt', text: 'Olá Mundo', encoding: 'utf-8')
        sh 'cat teste-file.txt'
      }
    }
  }
}