pipeline{
    agent any
    
    tools {
        gradle 'gradle'
    }
    
    stages{
        
        stage("Clone Repository"){
            steps{
            git branch: 'master', url: 'https://github.com/SherryObuhuma/java-todo'
        }
        }
        stage("Build Code"){
            steps{
                sh 'gradle build'
            }
        }
        stage("Test Code"){
            steps{
                sh "gradle test"
            }
        }
    }
}
