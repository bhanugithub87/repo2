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
        sh 'id'
        sh 'who'
        sh 'ls -ltra'
        sh './run-deployment.sh'

      }
    }
  
  }
  
}
