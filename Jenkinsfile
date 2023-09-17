pipeline{
    agent any
    tools { 
    gradle "gradle8.3"
  }
    stages{
        stage('clone Repo'){
            steps{
            git 'https://github.com/wanzetse/java-todo2'
            }
        }
        stage('Build Project'){
            steps{
            sh 'gradle build'
            }
        }
         stage('Test Project'){
            steps{
            sh 'gradle test'
            }
        }
         
    }
}
