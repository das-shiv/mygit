pipeline{

    agent any

    stages{
        stage("Fetch code from Githun"){
            steps{
            git branch: 'mater'; url: 'https://github.com/ss-das/mygit.git'
            }

        }

        stage("Deploy code to server"){
            steps{

            sh "mv /workspace/* /var/www/html/"
            }
        }

        post{
            echo "Sucessfully deployed"
        }
    
    }


}
