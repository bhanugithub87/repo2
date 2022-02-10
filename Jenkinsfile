pipeline {

  agent any
  parameters {
        string(name: 'clientjourneysvc',defaultValue:'svc1', description: 'backend version')
        string(name: 'clientjourneyui',defaultValue: 'ui1', description: 'frontend version')

    }
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
  
    stage('one'){
      steps{
        sh 'date'
        echo "backend: ${params.clientjourneysvc}"
        echo "frontend: ${params.clientjourneyui}"
        sh 'chmod a+x run-deployment.sh'
        sh "./run-deployment.sh"
        sh 'date'
      }

    }
  
  }
  
}
