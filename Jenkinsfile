#!groovy
branch = env.BRANCH_NAME

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
				script{
						echo "Script is executing now"
						echo "${branch}"
				}
			}			
		}

	}	
}
