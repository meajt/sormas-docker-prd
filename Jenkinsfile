node {

    stage('SCM checkout'){
        steps{
		script {
                    // Define your Git repository URL
                    def gitRepoUrl = 'https://github.com/meajt/sormas-docker-prd.git'
                    
                    // Checkout code from the 'np_change' branch
                    checkout([$class: 'GitSCM', branches: [[name: 'np_change']], userRemoteConfigs: [[url: gitRepoUrl]]])
                }

		}
    }
    stage('Compile-Package'){
        sh 'mvn clean install'
    }
        
}
