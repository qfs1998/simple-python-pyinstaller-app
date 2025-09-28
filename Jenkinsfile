pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'cd ~ && echo Build hello > hello_jenkins.txt'
            }
        }
        stage("Test"){
            steps{
                sh 'echo Test hello'
                sh 'echo Test world'
            }
        }
    }
}