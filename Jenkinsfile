pipeline {
    agent any
    stages {
        stage('build') {
            steps {
		cmd_exec('echo "Buils starting..."')	
		cmd_exec('echo "dir /a /b"')
		cmd_exec('java -version')
		cmd_exec('mvn -version')
            }
        }
	def cmd_exec(command) {
    	    return bat(returnStdout: true, script: "${command}").trim()
	}
    }
}