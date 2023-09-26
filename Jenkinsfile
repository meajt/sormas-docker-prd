node {

    stage('SCM checkout'){
        git branch: 'np_change',   url: 'https://github.com/meajt/SORMAS-Project.git'
    }
    stage('Compile-Package'){
        sh 'cd sormas-base'
        sh 'mvn clean -DskipTests=true install'
    }
        
}
