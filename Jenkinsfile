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
                sh 'lscpu'
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