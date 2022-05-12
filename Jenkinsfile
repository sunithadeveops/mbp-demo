pipeline{
  agent any
  stages{
    stage("Maven build"){
      when{
        branch 'feature'
      }
      steps{
          echo "maven build"
      }
    stage("sonar Analysis"){
      when{
        branch 'feature'
      } 
       steps{
          echo "sonar analysis"
       }
    }
    stage("deploy to dev"){
      when{
        branch 'develop'
      } 
       steps{
          echo "deploy to dev"
       }
    } 
    stage("deplot to qa"){
      when{
        branch 'test'
      } 
       steps{
          echo "deploy to qa"
       }
    }
    stage("deploy to product"){
      when{
        branch 'feature'
      } 
       steps{
          echo "deplot to prod"
       }
    }
  }
}
