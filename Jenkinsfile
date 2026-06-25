pipeline {
agent any

stages {

    stage('Checkout') {
        steps {
            echo 'Checkout Stage'
        }
    }

    stage('Docker Build') {
        steps {
            dir('app') {
                sh 'docker build -t moneyview-app .'
            }
        }
    }

    stage('Test') {
        steps {
            echo 'Testing Application'
        }
    }

    stage('Deploy') {
        steps {
            echo 'Deployment Started'
        }
    }
}

}
