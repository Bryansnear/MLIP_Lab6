pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '''
                echo In C or Java, we can compile our program in this step
                echo In Python, we can build our package here or skip this step
                '''
            }
        }
        stage('Test') {
            steps {
                bat '"C:/Users/bryan/AppData/Local/Programs/Python/Python312/python.exe" -m pytest'
            }
        }
        stage('Deploy') {
            steps {
                echo 'In this step, we deploy our project'
                echo 'Depending on the context, we may publish the project artifact or upload pickle files'
            }
        }
    }
}
