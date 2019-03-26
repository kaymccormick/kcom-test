pipeline {
    options { timeout(time: 10, unit: 'MINUTES') }
    agent { docker { image 'node:latest' } }
    stages {
        stage('build') {
            steps {
	    	sh 'mkdir -p kaymccormick-com'
		sh 'wget -O - -q https://jenkins.heptet.us/job/github/job/kaymccormick-com/job/master/lastSuccessfulBuild/artifact/build/kaymccormick-com.tar.gz | tar -zxf - -C kaymccormick-com'
            }
        }
    }
}