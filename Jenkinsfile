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
			
			 git branch: 'master',
                url: 'https://github.com/DipanGarg/ExtentReports.git'

            sh "ls -lat"
            sh 'mvn clean install'
			
			 git branch: 'master',
                url: 'https://github.com/DipanGarg/ExcelReader.git'

            sh "ls -lat"
            sh 'mvn clean install'
			
			 git branch: 'master',
                url: 'https://github.com/DipanGarg/Utilities.git'

            sh "ls -lat"
            sh 'mvn clean install'
			
			
			 git branch: 'master',
                url: 'https://github.com/DipanGarg/Selenium-Adapter.git'

            sh "ls -lat"
            sh 'mvn clean install'
			
			 git branch: 'master',
                url: 'https://github.com/gauravshukla01/Databse-Adapter.git'

            sh "ls -lat"
            sh 'mvn clean install'
			
			 git branch: 'master',
                url: 'https://github.com/gauravshukla01/Selenium-cucumber-Adapter-merged.git'

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
