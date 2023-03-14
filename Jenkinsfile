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
        steps{
          mail bcc: '', body: 'Job: ${env.JOB_NAME}\nBuild number :${env.BUILD_NUMBER}\n Build URL: ${env.BUILD_URL} ', cc: '', from: '', replyTo: '', subject: 'Testing purpose', to: ' saurabh29aws12sa@gmail.com'
        }
      }
    }//Results
  }//stages
}//pipeline
