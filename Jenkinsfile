@Library('brocode-libraries') _

pipeline{ 

    agent any

    stages{

        stage('Git Checkout'){

            steps{

                script{
                    
                    gitCheckout(
                        branch: "main"
                        url: " https://github.com/uday898989/brocode.git "
                    )

                     
                }
            }
        }
    }
}