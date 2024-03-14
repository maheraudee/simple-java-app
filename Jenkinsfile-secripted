node{
    git branch: 'main' , url: 'https://github.com/maheraudee/simple-java-app.git'
    stage('Build'){
        try{
            sh'echo "Building image stage"'
        }
        catch(Exception e){
            sh'esho "Exception found "'
            throw e
        }
    }
    stage('test'){
        if (env.BRANCH_NAME == "feature"){
            sh'echo "test stage"'
        }
        else {
            sh'echo "skip test stage"'
        }
    }
}