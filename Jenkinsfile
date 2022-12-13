pipeline {
  agent any
  stages {
    stage('Get Pods') {
        steps {
        echo 'Hello'
      }
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
