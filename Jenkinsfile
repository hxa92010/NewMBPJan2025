pipeline {
   agent any
   stages {
       stage('Build the  Code') {
           steps {
               sh "mvn clean package"
               echo "Building  Artifact for project samplewebapp"
			 
               
           }
       }
       stage('Reading branch wise info')
       {
       when
       {
       branch "feature*"
       }
       steps
       {
       echo " It is only for Feature branch"
       }
       }

       stage('Deploy  Code') {
	   
          steps {
               sh "mvn tomcat7:deploy"
               echo "Deploying Code"
			
               
          }
      }
      }
      }
