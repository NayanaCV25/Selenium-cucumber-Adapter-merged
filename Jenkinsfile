pipeline {
 
  agent {
        docker {
            image 'blackcatsolutions/maven-chrome-headless'
        }
    }

  stages {

    stage('Test') {

      steps{
       
        sh 'mvn --version'

        sh 'mvn test -D testng.xml'
        
      }

    }

  }

}
