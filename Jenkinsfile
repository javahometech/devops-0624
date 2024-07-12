pipeline{
  agent any
  stages {
    stage("SCM Checkout"){
      when {
          branch "develop"
      }
      steps{
        echo "Checking out from git"
      }
    }

    stage("Maven Build"){
      when {
          branch "develop"
      }
      steps{
        echo "Maven build finished"
      }
    }
    stage("Dev Deploy"){
      when {
          branch "develop"
      }
      steps{
        echo "Deploy to dev environment."
      }
    }
    stage("Prod Deploy"){
      when {
          branch "main"
      }
      steps{
        echo "Deploy to the production environment."
      }
    }
  }
}
