pipeline
{
    agent any
       tools{
        maven 'Maven 3.9.2'
    }
        stages{
            stage('Build Maven'){
                steps{
                 checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ziasix1nine/netCoreApp.git']])
                bat 'mvn clean install'
                }
            }
        }
}
