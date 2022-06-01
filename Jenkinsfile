pipeline{
    agent any
    stages{
        stage('stage1'){
            steps{
                echo "stage 1"
            }
        }
        stage('stage2'){
            steps{
                echo "stage 2"
            }
        }
        stages{
            stage('inner stage1'){
                steps{
                    echo "inner stage1"
                }
            }
        }
    }
}