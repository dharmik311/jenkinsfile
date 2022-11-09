pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('directory'){
            steps {
                echo(pwd())
            }
        }
        stage('input phase'){
            steps{
                input('Do you want to continue ?')
            }
           
        }
        stage('string parameter'){
            steps{
                echo ("$name")
            }
           
        }
        stage ('integrate phase'){
                when{
                 not{
                  branch "master"
                }
                }
            steps {
                echo 'Integration test passed'
               
                }
        }
       
        stage ('parellel '){
                steps{
                   input('do you want to procee further?')
                }
            }
   
           
           
       
       
       
               

    }
}
