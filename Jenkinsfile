pipeline {
    agent any
    stages{
        stage('build'){
            steps{
                bat 'mvn clean package'
                bat "docker build . -t tomcatwebapps:${env.BUILD_ID}"
            }
        }


    }

}
