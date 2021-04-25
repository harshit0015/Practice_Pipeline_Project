pipeline{
    agent any

    stages{
      
      stage("Branch") {
            steps {
                git branch: 'pipeline_1', url: 'https://github.com/harshit0015/Practice_Pipeline_Project.git'
            }
        }
        stage("Build"){
            steps{
                sh 'mvn clean compile'
            }
        }
        
        stage("Test"){
            steps{
                sh 'mvn test'
            }
        }
    }
}
