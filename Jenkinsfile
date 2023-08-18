@Library( 'brocode-library') _

pipeline{ 

    agent any
    
    parameters{
        choice( name: 'action', choices: 'create\ndelete', decription: 'Choose create/destroy')
    }

    stages{

        when { expression { params.action =='create' }}
        }

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

             when { expression { params.action =='create' }}

            steps{

                script{
                    
                    mvnTest()
                     
                }
            }
        }
    }
