pipeline {

  agent any
  parameters {
        string(name: 'clientjourneysvc',defaultValue:'svc1', description: 'backend version')
        string(name: 'clientjourneyui',defaultValue: 'ui1', description: 'frontend version')

    }
  stages {
  
    stage('one'){
      steps{
        
        echo "backend: ${params.clientjourneysvc}"
        echo "frontend: ${params.clientjourneyui}"
        sh 'chmod a+x run-deployment.sh'
        sh './run-deployment.sh'

      }
    }
  
  }
  
}
