pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh './test.sh' 
            }
        }
	stage('MySQL') {
	    steps {
		sh 'mysql -uroot -pmanai88 -B --exec="connect information_schema; select * from USER_PRIVILEGES"'
	    }
	}
    }
}
