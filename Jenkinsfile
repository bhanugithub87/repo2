#!groovy

def runScript(){
    echo 'script called'
    sh '''
    ls -la
    '''
 }

node{
  
 
    runScript()
     deleteDir()
     runScript()
     checkout scm
     runScript()
  
  
}
