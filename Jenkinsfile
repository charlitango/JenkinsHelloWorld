pipeline{
  agent any
  stages{
    stage('Parallel Execution'){
      steps{
        parallel(
          Build:{
            echo "Buil stage"
          }
          Test:{
            echo "Test stage"
          }
          Deploy:{
            echo "Deploy stage"
          }
        )
    }
  }
  }//stages
}//pipeline
