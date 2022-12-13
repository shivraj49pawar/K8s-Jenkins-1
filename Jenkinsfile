pipeline {
  agent kubernetes
  stages {
    stage('Get Pods') {
      steps {
        sh 'kubectl get pods'
      }
    }

  }
  environment {
    KUBECONFIG = '/var/lib/jenkins/kube.config'
  }
}
