pipeline
{
    agent any 
    
    triggers { cron('H */4 * * 1-5') }
    
 parameters { choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '') }
    
    stages{
        
        stage("build"){
            steps{
                echo "hello from build"
            }
            
        }
        stage("test"){
            steps{
                echo "hello from test"
            }
            
        }
    }
    
    
    
}
