#!groovy
branch = env.BRANcH_NAME

pipeline
{
	agent any
	stages
	{
		stage('clean')
		{
			steps
			{
				deleteDir()
				echo "Cleaning completed"
			}
			
		}

		stage('Checkout')
		{
			steps
			{
				checkout scm
				echo "Cloning the latest code from GitHub"
				echo "${branch}"
			}			
		}

	}	
}
