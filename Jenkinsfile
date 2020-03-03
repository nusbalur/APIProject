node {
        stage('Checkout') {
            git url: 'https://github.com/nusbalur/APIProject.git/my-folder',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       
			
	stage('Build') {
		def mvn_version = 'soapui_maven'
		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {
			sh 'mvn site'
			}
		}
}
