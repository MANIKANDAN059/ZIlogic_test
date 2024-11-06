pipeline{
    agent any
	stages{
		stage('build') {
    		steps {
        		sh 'ls'
        		sh 'python test_app.py'
    		}
		}

		stage('read') {
        	steps {
        		script {
                   def data = readFile(file: 'sample_data.txt')
                   println(data)
               }
           }
       }
	}
}
