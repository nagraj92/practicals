pipeline {
    agent {
      label 'node-1'
    }
    options{
        timeout(time: 4,unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {
        stage('Build') {
            steps {
                echo 'build ra'
                sh 'sleep 23'
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
