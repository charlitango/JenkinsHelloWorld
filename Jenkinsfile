pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo "Building"
      }
    }//Build
    stage('Test'){
      steps{
        echo "Testing"
      }
    }//Test
    stage('Deploy'){
      steps{
        echo "Deploying"
      }
    }//Deploy
    stage('Email'){
      steps{
        input("Do you need send email?")
      }
    }//Results
  }//stages
}//pipeline
