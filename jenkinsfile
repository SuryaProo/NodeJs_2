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
                sh 'sudo yum install npm'
                sh 'sudo npm test'
            }
        }
        
        stage("Build"){
            steps{
                sh 'npm run build'
            }
        }
    }
}
