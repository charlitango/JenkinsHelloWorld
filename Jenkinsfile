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
    stage('Consolidate results'){
      steps{
        input("Do you need to capture results?")
        junit '**/target/surefire-reports/Test-*.xml'
        archive 'target/*.jar'
      }
    }//Results
  }//stages
}//pipeline
