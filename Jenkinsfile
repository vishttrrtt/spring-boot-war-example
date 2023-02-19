pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
    stages {
        
        stage('scm checkout') {
            steps {
               checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sudhakarbastawade2303/spring-boot-war-example.git']]) 
            }
        }
        stage('build the scm') {
            steps {
                sh 'mvn install'
            }
        }
        stage('deploy to tomcat server') {
            steps {
                sh 'mvn install'
            }
        }
    }
}




