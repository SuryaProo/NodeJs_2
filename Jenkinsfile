pipeline{
    agent any
    
    stages{
        stage("checkout"){
            steps{
                git branch: 'main', url: 'https://github.com/SuryaProo/NodeJs_2.git'
            }
        }
        
        stage("test"){
            steps{
                sh 'sudo -S yum install npm -y'
                sh 'sudo -S npm test'
            }
        }
        
        stage("Build"){
            steps{
                sh 'npm run build'
            }
        }
    }
}
