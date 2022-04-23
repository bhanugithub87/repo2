#!groovy

properties([parameters([string('empno')])])
def empno
def names = ['one','two','three']

try{
    
    node{
    
        stage('build...'){
            
            println names.getClass()
            echo params.empno
            nameExists = params.empno in names
            if(nameExists){
                echo 'true case'
            }else{
                echo 'false case'
            }
            echo '************'
            sh '''
            printenv
            '''
            echo 'done'
                
            
        }
        
    }

} catch(e){
echo 'in catch'
    println e
}
