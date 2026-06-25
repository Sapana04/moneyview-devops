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
            sh 'docker rm -f moneyview-container || true'
        sh 'docker run -d -p 3000:3000 --name moneyview-container moneyview-app'
        }
    }
}

}
