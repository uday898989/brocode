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
         
         stage('static code analysis: sonarqube'){

            steps{
               script{
                   
                   statiCodeAnalysis()
               }
            }
        }
         
        
    
    }
}