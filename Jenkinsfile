pipeline{
    agent any
    stages{
        stage('stage1'){
            steps{
                echo "stage 1"
            }
        }
        stage('stage2'){
            stages{
                        stage('inner stage1'){
                            steps{
                                echo "inner stage1"
                            }
                        }
                    }
        }
        stage('parallel'){
            parallel{
                stage('parallel-1'){
                    echo "parallel-1......."
                }
                stage('parallel-2'){
                    echo "parallel-2......."
                }
            }
        }
    }
}