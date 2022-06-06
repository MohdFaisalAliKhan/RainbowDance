pipeline{
    agent any{
        stages{
          stage('One'){
            steps{
                echo "Hello this is faisal"
            }
          }
          stage('Two'){
            steps{
               input("Do you want to proceed?")
            }
          }
          stage('Three'){
            when{
              not{
                 branch "master"
              }
            }
            steps{
                echo "Master branch not ditected."
            }
          }
        }
    }

}
