pipeline{
agent any
  stages {
    stage("build &test")
    when {
      branch "develop"
    steps{
      echo"building & testing app"
    }
  }
   stage(" dev deploy")
    when {
      branch "develop"
    steps{
      echo"deploy to dev env"
}
}
    stage(" dev test ")
    when {
      branch "test"
    steps{
      echo"deploy to test deploy"
  }
}
     stage(" dev prod ")
    when {
      branch "main"
    steps{
      echo"deploy to test deploy"
  }
    }
  }
}
