pipeline{
    agent any
    stages{
        stage('1-repoclone'){
            steps{
                sh 'df -h'
            }
        }
        stage('2-cpuanalysis'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-id', url: 'https://github.com/ukasamgithub/team4-pipeline-dm.git']])
            }
        }
        stage('3-memorycheck'){
            steps{
                sh 'free -g'
            }
        }
        stage('4-os-stats'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
        stage('5-welcomemassage'){
            steps{
                echo "welcome to pipeline as a code"
            }
        }
    }
}