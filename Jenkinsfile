pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ PES2UG20CS367_TanyaArora.cpp -o PES2UG20CS367'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS367'
    }
  }

  stage('Deploy') {
//     steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
