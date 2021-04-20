pipeline
{
agent any
stages{
stage {"Build Application"}{
steps{
sh mvn clean install 
	}
	}

stage {"Deploy Application to Cloudhub"}{
steps{
sh mvn package deploy -DmuleDeploy 
}
}
}
}