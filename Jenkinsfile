 pipeline{
    agent any
    stages{
        stage('build'){
           steps{
            echo "initial build"
           } 
        }

        stage('scan'){
            steps{
                echo "scanning the app"
            }
        }
        stage('docker builld'){
            steps{
                echo "docker"
            }
        }
        stage('deploy to dev'){
            steps{
                echo "dev"
            }
        }
        stage('deploy to test'){
            steps{
                echo "test"
            }
        }

        stage('deploy to prod'){
            input {
                message "ready to deploy to prod ?"
                ok "yes"
                submitter "TAMILTECH,kunju"
            }
            steps{
                echo "prod"
            }
        }
    }
}
