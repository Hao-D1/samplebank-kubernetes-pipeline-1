node {	
      stage('DeployProduction') {
         // first we clean production        
         echo 'Build loading'
         dir ('deployment-files')
	    {
		    kubeconfig(credentialsId: 'kube-config', serverUrl: '') {
				 sh 'kubectl get all --all-namespaces'
			 }		   
		   echo 'build completed'
         }
    }        
}
