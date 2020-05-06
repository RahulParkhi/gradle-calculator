pipeline
{
agent any
     stages
     {
	  stage ('download the source code from SCM')
          {
          	steps
      		{
        		git branch: 'master', url: 'https://github.com/RahulParkhi/gradle-calculator.git'
      		}
    	  }
	  stage("Run Gradle command")
	  {
               steps
	       {	
                    withGradle
		       {
    				sh 'gradle build --info'
		       }
               }
          }
     }
}
