#!groovy

properties([parameters([string('empno')])])
def empno
def names = ['one','two','three']
def nameExists;
try{
    
    node{
    
        stage('build...'){
            
            println names.getClass()
            nameExists = 'two' in names
            echo nameExists
                
            
        }
        
    }

} catch(e){
echo 'in catch'
}
