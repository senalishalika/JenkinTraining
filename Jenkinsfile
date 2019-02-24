node{
    stage('SCM Checkout'){
        
        git 'https://github.com/senalishalika/JenkinTraining'
    }
    stage('Initialize'){
        def dockerHome = tool 'myDocker'
        def mavenHome  = tool 'myMaven'
        env.PATH = "${dockerHome}/bin:${mavenHome}/bin:${env.PATH}"
        
    }
     stage('Compile Stage'){
         def mavenHome  = tool 'myMaven'
         echo "${mavenHome}/bin/mvn clean compile"
    }
   
}
