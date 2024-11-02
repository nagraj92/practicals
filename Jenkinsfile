pipeline {
    agent {
      label 'node-1'
    }
    options{
        timeout(time: 1,unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                echo 'build ra'
                sh 'sleep 10'
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
