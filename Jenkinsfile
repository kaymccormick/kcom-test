pipeline {
    options { timeout(time: 10, unit: 'MINUTES') }
    agent { docker { image 'node:latest' } }
    stages {
        stage('build') {
            steps {
		sh 'wget https://jenkins.heptet.us/job/github/job/kaymccormick-com/job/master/lastSuccessfulBuild/artifact/build/kaymccormick-com.tar.gz'
            }
        }
    }
}