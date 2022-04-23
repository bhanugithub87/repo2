#!groovy

def runScript(){
    echo 'script called'
    sh '''
    ls -la
    '''
 }


node{
    
    
properties([buildDiscarder(logRotator(numToKeepStr: '4')), parameters([string(name: 'empnumber')])])
  
 
    runScript()
     deleteDir()
     runScript()
     checkout scm
     runScript()
  
  
}
