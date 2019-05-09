pipeline {
 
  agent {
        docker {
            image 'blackcatsolutions/maven-chrome-headless'
        }
    }

  stages {

    stage('Test') {
        steps {
            git branch: 'master',
                url: 'https://github.com/DipanGarg/ConfigProvider.git'

            sh "ls -lat"
            sh 'mvn clean install' 
          
        }
     
  /*    steps{
       
        sh 'mvn --version'

        sh 'mvn test -D testng.xml'
        
      } */

    }

  }

}
