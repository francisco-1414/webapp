pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hola'
        sh 'mvn package'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('Deliver') {
      steps {
        sh '.\\contenedores\\python'
      }
    }

  }
}