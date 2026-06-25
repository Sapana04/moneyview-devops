pipeline {
agent any

```
stages {

    stage('Checkout') {
        steps {
            git branch: 'main',
            url: 'https://github.com/Sapana04/moneyview-devops.git'
        }
    }

    stage('Build') {
        steps {
            echo 'Build Started'
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
```

}
