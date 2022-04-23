node{
  
  def runScript(){
    echo 'script called'
    sh '''
    ls -la
    '''
  
  }

  stage('build'){
    runScript
  }
  
}
