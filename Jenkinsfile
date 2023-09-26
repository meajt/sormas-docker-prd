node {

    stage('SCM checkout'){
        git branch: 'devops',   url: 'https://github.com/meajt/sormas-docker-prd.git'
    }
    stage('Compile-Package'){
        sh 'mvn clean install'
    }
        
}
