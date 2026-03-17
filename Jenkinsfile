pipeline{
    agent{
        label 'linux_node'
    }
    stages{
        stage('Compile'){
            steps{
                echo "compiling the code"
            }
        }
        stage('code review'){
            steps{
                echo "Reviewing the code"
            }
        }
        stage('test'){
            steps{
                echo "testing the code"
            }
        }
        stage('Coverage analysis'){
            steps{
                echo "code coverage analysis"
            }
        }
        stage('Package'){
            steps{
                echo "packaging the code"
            }
        }
    }
}