[200~pipeline {
       agent {
	       label {
		       label "built-in"
			   customWorkspace "/mnt/project"
		   }
	   }
	   
	   stages { 
	       stage ( 'mkdir-1') {
		        steps {
				     sh "rm -rf *"
					 sh "mkdir test-folder-1"
				}
		   }
		   
		   stage ('mkdir-2') {
		         steps {
				      dir ("/mnt/data/wsp-2") {
					         sh "rm -rf"
					         sh "mkdir test-folder-2"
					  }
				 }
		   }
		    stage ('mkdir-3') {
		         steps {
				      dir ("/mnt/data/wsp-3") {
					         sh "rm -rf" 
					         sh "mkdir test-folder-3"
					  }
				 } 
		   }
		   stage ('mkdir-4') {
		         steps {
				      dir ("/mnt/data/wsp-4") {
					          sh "rm -rf"
					         sh "mkdir test-folder-4"
					  }
				 } 
		   }
		   
	   }
}
