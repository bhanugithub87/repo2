#!groovy

def runScript(){
    echo 'script called'
    sh '''
    ls -la
    '''
 }

node{
  
 stage('build'){
    runScript()
     deleteDir()
     runScript()
     checkout scm
     runScript()
  }
  
}
