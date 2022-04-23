#!groovy

properties([parameters([string('empno')])])
def empno
try{
    
    node{
    
        stage('build...'){
            
            empno = params.empno as int
            
                if(empno == 100){
                    echo 'empno is hundred'
                }else{
                    echo 'empno is not hundred'
                }
                
            
        }
        
    }

} catch(e){
echo 'in catch'
}
