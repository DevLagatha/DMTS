pipeline {
  agent {
    kubernetes {
      label 'simple-test'
      yamlFile 'pod.yaml'
    }
  }
  stages {
    stage('Check Python') {
      steps {
        container('python') {
          sh 'python --version'
        }
      }
    }
  }
}
