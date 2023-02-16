pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o task5 new.cpp'
        build job: 'PES1UG20CS203-1'
      }
    }
    stage('Test'){
      steps{
        sh './task5'
      }
    }
   stage('Deploy'){
      steps{
        echo 'Deploying'

      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
