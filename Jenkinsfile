pipeline{
  agent any
  stages{
    stages("Build"){
      steps{
        echo "Building ..."
        }
        post{
          always{
            mail to: "fernandojanuda@gmail.com",
            subject: "Build Status Email",
            body: "Build log attached!"
          }
      }
    }
    stage("Test"){
      steps{
        echo "Testing ..."
      }
    }
    stage{"Deploy"){
      steps{
        echo "Deploying ..."
      }
    }
  }
}
