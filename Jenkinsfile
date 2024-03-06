pipeline {
    agent any
    stages {
//          stage('Clone repository') {
//              steps {
//                  checkout ([Sclass: 'GitSCM',
//                    branches: [[name:*/main']],
//                    userRemoteConfigs: [[url: 'https://github.com/mehtasaransh11/PES1UG21CS538_Jenkins/']]])
//              }
//          }
          stage('Build') {
              steps {
                  build 'PES1UG21CS538-1'
                  sh g++ main. cpp -o output'
              }
        }
        stage('Test') {
            steps {
                sh './output'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'deploy'
            }
        }
    ｝
    post{
        failure{
            error 'Pipeline failed'
        }
    }
｝
