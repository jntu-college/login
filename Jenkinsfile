#!groovy
branch = env.BRANH_NAME

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
				echo "branch Name is: ${branch}"
			}			
		}

	}	
}
