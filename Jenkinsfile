pipeline
{
agent any
	environment {
	PATH = "$PATH:/opt/apache-maven-3.6.3/bin"
	}
  stages{
    stage('GetCode'){
      steps{
        git 'https://github.com/Shivamgupta18/maven-web-app.git' 
      }
    }
    stage('Build'){
      steps{
       sh 'mvn clean package' 
      }
    }
  }   
}
