pipeline {
  agent {
    node {
      label 'cloudfoundry'
    }
    
  }
  stages {
    stage('Development') {
      steps {
        pushToCloudFoundry(organization: 'Releng-Devops', target: 'https://api.run.pivotal.io', cloudSpace: 'development', credentialsId: '45e1ad8c-3b41-4eeb-b564-d2e92617f1a2', pluginTimeout: 60)
      }
    }
  }
}