pipeline {
  agent any
  environment {
  KUBECONFIG = '/var/lib/jenkins/kube.config'
  }
  stages {
    stage('Get Pods') {
      steps {
        sh 'kubectl get pods'
      }
     

  }
}
