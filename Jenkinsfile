pipeline{
    agent any 
    stages{
      stage('1-git clone'){
        steps{
       checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'NanjeD', url: 'https://github.com/NanjeD/jenkins_jobs.git']])
        }
      }
      stage('2-system check'){
        steps{
          sh ' echo "walk...." '
          sh 'lscpu'
        }
      }
      stage('3-memory check'){
        steps{
          sh ' echo "walk...." '
          sh 'cat /etc/passwd | grep ubuntu'
        }
      }
      stage('4-os stats'){
        steps{
          sh ' echo "walk...." '
          sh 'whoami'
        }
      }
      stage('5-o system analysis'){
        steps{
          sh ' echo "The final level"'
          sh 'pwd'
        }
      }
      stage('6-webhook testing'){
        steps{
          sh ' echo "walk...." '
          sh 'ps -ef'
        }
      }
      stage('7-the seventh steps'){
        steps{
            sh 'whoami'
        }
      }
      stage('security check'){
        steps{
            sh 'bash -x /var/lib/jenkins/workspace/demo-groovy/security.sh'
        }
      }
    }
  }
