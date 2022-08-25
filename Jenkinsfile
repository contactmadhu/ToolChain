pipeline {
    agent any 
   tools {
        maven 'maven'
     jdk 'jdk11'
    }
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world! from Bit Bucket' 
                echo 'added webhook and IP to security group'   
                echo 'Configured plugins on Jenkins'
                echo 'Changed version of BitBucket'
                echo 'Changed to plugin from native on jenkins for  BitBucket'
                echo 'Add behaviour on jenkins - over ride hook'
                echo 'upgarde creds'
                echo 'new webhook plugin'
                echo ' Webhook to Jenkins for Bitbucket Server on bitbucket'
                echo ' Added Sonar'
            }
        }
          stage ('Build') {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
            post {
                success {
                    junit 'target/test-results/**/*.xml' 
                }
            }
        }
    }
}   