pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        writeFile(file: 'teste-file.txt', text: 'Olá Mundo', encoding: 'utf-8')
        sh 'cat teste-file.txt'
      }
    }
    stage('Verificar') {
      steps {
        input(message: 'Deseja continuar?', id: 'check', ok: 'Sim')
      }
    }
    stage('Mensagem Final') {
      steps {
        echo 'Fim'
      }
    }
  }
}