pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue: 'XYZ', description: 'A string parameter')
        booleanParam(name: 'STATUS', defaultValue: true, description: 'Please select the status')
        choice(name: 'BROWSER', choices: ['Firefox', 'Chrome', 'Edge'], description: 'Please select the browser for execution')
        password(name: 'PASSWORD', defaultValue: 'password123', description: 'Please enter password')
        file(name: 'MY_FILE', description: 'A file parameter')
    }

    stages {
        stage('Print Parameters') {
            steps {
                script {
                    echo "USERNAME: ${params.USERNAME}"
                    echo "PASSWORD: ${params.PASSWORD}"
                    echo "STATUS: ${params.STATUS}"
                    echo "BROWSER: ${params.BROWSER}"
                    echo "MY_FILE: ${params.MY_FILE}"
                }
            }
        }
    }
}
