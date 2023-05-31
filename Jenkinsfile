pipeline
{
    agent any
       tools{
        maven 'Maven -X'
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
