pipeline {
    agent {
        label 'ubuntu-agent'
    }

    parameters {
        string(
            name: 'USER_NAME',
            defaultValue: 'Matan',
            trim: true,
            description: 'Enter your name'
        )

        booleanParam(
            name: 'RUN_TEST',
            defaultValue: true,
            description: 'Run tests?'
        )

        choice(
            name: 'ENVIRONMENT',
            choices: ['development', 'staging', 'production'],
            description: 'Choose environment'
        )
    }

    stages {
        stage('Verify Agent') {
            steps {
                sh 'hostname'
                echo "Hello ${params.USER_NAME}"
                echo "Environment: ${params.ENVIRONMENT}"
            }
        }
    }
}