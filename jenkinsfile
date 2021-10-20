
pipeline{
  stages{
    stage("checkout"){
      steps{
        Scripts{
	  checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'java-mavan-project-repo', url: 'https://github.com/sriram-naresh/java-maven-project.git']]])
	  }
        }
     }
   }
 }
