pipeline{
    agent {
        label 'slave'
    }
    tools{
        maven 'maven'
    }
    stages{
        stage('checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/RamanaMedaraboina/rams2.git'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean verify'
            }
        }
    }
}