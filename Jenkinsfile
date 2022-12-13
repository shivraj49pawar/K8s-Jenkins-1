pipeline {
  agent any
  stages {
    stage('Get Pods') {
      steps {
        sh 'kubectl apply -f pods.yml' 
        sh 'kubectl get pods'
      }
    }

  }
  environment {
    KUBECONFIG = '/var/lib/jenkins/kube.config'
  }
}
