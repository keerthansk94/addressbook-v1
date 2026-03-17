pipeline{
    agent{
        label 'linux_node'
    }
    parameters{
        string(name:'Env' , defaulyValue: 'Test', description : 'Enviroment name' )
        booleanParam(name: 'executeTests', defaultValue: true, description: 'decise to run test')
        choice(name: 'APPVERSION', choices: ['1,1','1.2','1.3'], description:'app version selection')
    }
    stages{
        stage('Compile'){
            steps{
                echo "compiling the code"
                sh 'mvn compile'
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