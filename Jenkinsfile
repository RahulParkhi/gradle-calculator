pipeline
{
agent any
     stages
     {
          stage("SCM Checkout")
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
