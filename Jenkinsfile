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
					echo '=========================='	
				}
			}
		}
	}
}