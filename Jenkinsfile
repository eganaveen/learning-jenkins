pipeline{
    agent any
    matrix{
        axes{
           axis{
              name 'PLATFORM'
              values 'linux','mac','windows'
           }
        }
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
                        steps{
                            echo "parallel-1......."
                        }
                    }
                    stage('parallel-2'){
                        steps{
                            echo "parallel-2......."
                        }
                    }
                    stage('parallel-3'){
                         steps{
                            echo "parallel-3......."
                        }
                    }
                }
            }
        }
    }
}