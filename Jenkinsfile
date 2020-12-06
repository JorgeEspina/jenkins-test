node {
    stage('Checkout SCM') {
        git branch: 'jenkins_test', url: 'https://github.com/JorgeEspina/jenkins-test.git'
    }

    stage('Install node modules') {
        sh "npm install"
    }

    stage("Test") {
        sh "npm run test-headless"
    }

    stage("Build") {
        sh "npm run build --prod"
    }
    
    stage("Copy") {
        
    }
}
