
pipeline{
agent  any
  stages{
    stage("checkout"){
      steps{
	checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sriram-naresh/java-maven-project.git']]])
	  }
        }
	  stage("build"){
	   steps{
	     script{
		sh """
		mvn clean
		mvn install
		"""
	     }
	   }
	  }
     }
}

