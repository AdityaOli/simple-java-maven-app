pipeline{
	agent any
	stages 
	{
		stage ('Compilation Stage') 
		{
			steps
			{
				withMaven(maven : 'maven_3_5_0')
				{
					bat 'mvn clean install'	
				}
			}
		}
		stage ('Testing Stage')
		{
			steps
			{
				withMaven(maven : 'maven_3_5_0')
				{
					bat 'mvn test'	
				}
			}
		}
		stage ('Deployment Stage')
		{
			steps
			{
				withMaven(maven : 'maven_3_5_0')
				{
					bat 'mvn deploy'	
				}
			}
		}
	}
}