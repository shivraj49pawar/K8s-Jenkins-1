pipeline {
  agent any
  stages {
    stage('Get Pods') {
      steps {
        sh 'kubectl apply -f pods.yaml' 
        sh 'kubectl get pods'
      }
    }

  }
  environment {
    KUBECONFIG = '/var/lib/jenkins/kube.config'
  }
}
