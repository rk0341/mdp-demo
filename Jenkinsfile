pipeline{
    agent any
    stages{
     stage ("maven build") {
         when{
             branch 'develop' 
         }
     steps{
     echo "maven build.."
      }
     }
       stage ("Sonar Analysis") {
         when{
             branch 'develop' 
         }
     steps{
     echo "Sonar Analysis.."
      }
     }
        stage ("Deploy to Dev") {
         when{
             branch 'develop' 
         }
     steps{
     echo "deploy to devlopment branch.."
      }
     } 
         stage ("Deploy to Qa") {
         when{
             branch 'test' 
         }
     steps{
     echo "deploy to Qa"
      }
     } 
         stage ("Deploy to Prod") {
         when{
             branch 'main' 
         }
     steps{
     echo "deploy to production.."
      }
     }  
    }
}
