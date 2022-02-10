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
        sh '''
        echo "${params.clientjourneysvc}"
        echo "two"
        '''
        sh 'date'
      }

    }
  
  }
  
}
