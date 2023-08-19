@Library('brocode-yt') _

pipeline{

    agent any


    stages{
         
        stage('Git Checkout'){
                    
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/uday898989/brocode.git"
            )
            }
        }
         stage('Unit Test maven'){
         
         

            steps{
               script{
                   
                   mvnTest()
               }
            }
        }
         
        
    
    }
}