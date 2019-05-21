//pipeline{
  //  agent any
//    stages{
        //stage('Build'){
        //    steps{
                //sh 'mvn clean package'
                //sh 'docker build . -t tomcatwebapp:(($env.BUILD_ID))
      //      }
    //    }
  //  }
//}


pipeline
{
    agent any
    
    stages
    {
        stage('Compile')
        {
            steps
            {
                withMaven(maven : 'localMaven')
                {
                    sh 'mvn clean package'
                }
                
            }
        }
        
    }
}
