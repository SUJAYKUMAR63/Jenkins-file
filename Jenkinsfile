pipeline
{
    agent {
    docker 
        {
        image 'maven'
        }
    } 
    
    triggers { cron('H */4 * * 1-5') }
    
 parameters { choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '') }
    
    stages{
        
        stage("build"){
            steps{
                sh 'mvn -version'
            }
            
        }
        stage("test"){
            steps{
                echo "hello from test"
            }
            
        }
    }
    
    
    
}
