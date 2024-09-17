pipeline{
	agent any
	stages{
		stage("Checkout"){
			steps{
				checkout scm
				}
			}
		stage("Build"){
			steps{
			sh '/home/pratikkambl3/Documents/Devops-Tools/apache-maven-3.9.9/bin/mvn install'
				}
			}
		stage("Deployment"){
			steps{
			sh 'cp target/Nike.war /home/pratikkambl3/Documents/Devops-Tools/apache-tomcat-9.0.93/webapps'
				}
			}
		}
	}
