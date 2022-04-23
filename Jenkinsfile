#!groovy

def runScript(){
    echo 'script called'
    sh '''
    ls -la
    '''
 }

properties([buildDiscarder(logRotator(numToKeepStr: '4')), parameters([string(description: 'employee num', name: 'empno')])])

node{
  
 
    runScript()
     deleteDir()
     runScript()
     checkout scm
     runScript()
  
  
}
