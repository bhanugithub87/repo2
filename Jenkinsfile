#!groovy

properties([parameters([string('empno')])])
def empno
try{
    
    node{
    
        stage('build...'){
            
            empno = params.empno
            println empno
            
        }
        
    }

} catch(e){
echo 'in catch'
}
