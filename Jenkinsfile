pipeline{
    agent any

  tools{
  maven "M3"
  }
  
    stages{
        stage('build'){
            steps{
                sh 'bash setup.sh'
                sh 'ls'
            }
        }
        stage('test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('deploy'){
            steps{
                sh 'mvn run'
            }
        }
    }
}
