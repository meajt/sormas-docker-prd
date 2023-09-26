node {

    stage('SCM checkout'){
        git branch: 'np_change',   url: 'https://github.com/meajt/SORMAS-Project.git'
    }
    stage('Compile-Package'){

        steps{
            dir('/var/lib/jenkins/workspace/sormas-prd/sormas-base'){
                sh 'mvn clean -DskipTests=true install'
            }
        }
        //sh 'cd sormas-base'
        //sh 'mvn clean -DskipTests=true install'
    }
        
}
