pipeline {
   agent any
    tools{
        maven 'Maven_3_9_2'
    }
    stages{
        stage('Build Maven')
        steps{
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ziasix1nine/netCoreApp.git']]])
                sh 'mvn clean install'
        }
    }
}
