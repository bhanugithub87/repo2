#!groovy

properties([parameters([string('empno')])])
def empno
def names = ['one','two','three']
def nameExists;
try{
    
    node{
    
        stage('build...'){
            
            println names.getClass()
            nameExists = 'two' in params.empno
            if(nameExists){
                echo 'true case'
            }else{
                echo 'false case'
            }
            echo 'done'
                
            
        }
        
    }

} catch(e){
echo 'in catch'
    println e
}
