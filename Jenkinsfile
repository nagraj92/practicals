pipeline {
    agent {
      label 'node-1'
    }
    options{
        timeout(time: 4,unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {
                echo 'build ra'
                sh 'sleep 23456789876'
            }
        }
        stage('Test') {
            steps {
              echo 'test ra'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy ra'
            }
        }
    }
}
