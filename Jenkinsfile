node('nodejs'){
    stage('Checkout'){
        git  branch: 'main',
             url: 'https://github.com/mrizwan93/do400-pipelines-control'
    }
    stage('backend test'){
        sh 'node ./backend/test.js'
    }
    stage('frontend test'){
        sh 'node ./frontend/test.js'
    }
}
