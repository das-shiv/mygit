pipeline{
    agent any
   
    stages{
        stage('Fetch code'){
            steps{
                git branch: 'master', url:'https://github.com/ss-das/mygit.git'

            }

        }
        stage('Put the code in apache server'){
            steps{
                
                sh 'sudo mv /var/lib/jenkins/workspace/GitPipeline/* /var/www/html/'
            }
        }
    }
}
