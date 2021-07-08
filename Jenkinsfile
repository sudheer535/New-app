git pipeline{
    agent {
        label 'Linux'
    }
    tools {
        maven 'Maven3'
    }
    stages{
        stage ('git checkout'){
            steps{
                git credentialsId: 'NewGitHub', url: 'https://github.com/sudheer535/New-app.git'
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn clean package'
            }
        }
        
    }
}
