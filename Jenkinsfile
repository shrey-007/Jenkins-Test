pipeline{
    agent any

    stages{
        stage("compile"){
            steps{
                bat 'javac Main.java'
            }
            
        }
        stage("run"){
            steps{
                bat 'java Main'
            }
            
        }
    }
// This is post build acions
    post{
        always{
            bat 'echo "This will run always"'
        }
        success{
            bat 'echo "This will run when build is successfull"'
        }
        failure{
            bat 'echo "This will run when build is a failure"'
        }
    }

}