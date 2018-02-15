pipeline {
  agent none
  stages {
    stage('Development') {
      steps {
        pushToCloudFoundry(organization: 'Releng-Devops', target: 'https://api.run.pivotal.io', cloudSpace: 'development', credentialsId: 'adew1@xl.co.id')
      }
    }
  }
  environment {
    Development = 'DEV'
  }
}