pipeline {
    agent any

    parameters {
        string(name: 'BUILD_NUMBER_INPUT', defaultValue: '1', description: 'Enter the build number')
    }

    stages {
        stage('Build') {
            when {
                branch 'development'
            }
            steps {
                echo "Running build on development branch"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying Build Number: ${params.BUILD_NUMBER_INPUT}"
            }
        }
    }
}
