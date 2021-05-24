pipeline{
    agent{
        node{
            label 'nodejs'
        }
    }

    stages{
        stage('Run Tests'){
            parallel{
                stage('Backend test'){
                    steps{
                        sh 'node ./backend/test.js'
                    }
                }
                stage('Frontend test'){
                    steps{
                        sh 'node ./frontend/test.js'
                    }
                }
            }
        }
    }
}
