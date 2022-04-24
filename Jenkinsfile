pipeline {
    agent any
    tools {nodejs "mynodejs"}
    stages {
        stage('Dev') {
            steps {
              git 'https://github.com/tejaspatane/aws_codebuild_codedeploy_nodeJs_demo.git'
              echo "the content as follows"
              sh 'cat index.js'
            }
        }
         stage('build') {
            steps {
                sh 'npm install'
            }
        }
    }
}