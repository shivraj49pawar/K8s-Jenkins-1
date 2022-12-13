pipeline {
  agent any
  stages {
     stage('Test_echo') {
      steps {
        echo 'Hello'
      }
    }
    stage('Get Pods') {
      steps {
        sh 'kubectl apply -f pods_wp.yml' 
        sh 'kubectl get pods'
      }
    }

  }
  environment {
    KUBECONFIG = '/var/lib/jenkins/kube.config'
  }
}
