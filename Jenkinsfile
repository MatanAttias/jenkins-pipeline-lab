pipeline{
    agent {
    label 'ubuntu-agent'
    }

    parameters {
        string(
            name: 'USER_NAME',
            defaultvalue: 'Matan',
            trim: true,
            description: 'Enter your name'
        )

        booleanParam(
            name: 'RUN_TEST',
            defaultvalue: true,
            description: 'Run tests?'
        )

        choice(
            name: 'ENVIRONMENT',
            choices: ['development', 'staging', 'production'],
            description: 'Choose environment'
        )




    }





}