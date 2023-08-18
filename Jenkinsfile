@Library( 'brocode-library') _

pipeline{ 

    agent any

    stages{

        stage('Git Checkout'){

            steps{

                script{
                    
                    gitCheckout(
                branch: "main",
                url: "https://github.com/uday898989/brocode.git"
            )
                     
                }
            }
        }
        stage('Unit Test maven'){

            steps{

                script{
                    
                    mvnTest()
                     
                }
            }
        }
        stage ('Integration Test maven'){

            steps{

                script{
                    
                    mvnIntegrationTest()
                     
                }
            }
        }
    }
}