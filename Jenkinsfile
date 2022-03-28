
pipeline{
agent  any
  stages{
    stage("checkout"){
      steps{
	 checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'gitcrends', url: 'https://github.com/sriram-naresh/java-maven-project.git']]])
	  }
        }
     }
}

