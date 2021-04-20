pipeline
{
agent any
stages{
stage ('Build Application'){
steps{
sh "export M2_HOME=/Users/abhijeetghatol/Downloads/apache-maven-3.8.1 # your Maven home path
export PATH=$PATH:$M2_HOME/bin
mvn clean install"
	}
	}

stage ("Deploy Application to Cloudhub"){
steps{
sh "export M2_HOME=/Users/abhijeetghatol/Downloads/apache-maven-3.8.1 # your Maven home path
export PATH=$PATH:$M2_HOME/bin
mvn package deploy -DmuleDeploy" 
	}
	}
}
}