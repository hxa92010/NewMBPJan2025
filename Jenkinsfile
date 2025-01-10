pipeline {
   agent any
   stages {
       stage('Build the   Code') {
           steps {
               sh """
               echo "Building  Artifact for project samplewebapp"
			   """
               
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

       stage('Deploy Code') {
	   
          steps {
               sh """
               echo "Deploying Code"
			   """
               
          }
      }
      }
      }
