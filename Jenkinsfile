@Library('company-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Using Shared Library') {
            steps {
                script {
                    buildApp('MyWebApp')
                    testApp('MyWebApp')
                    deployApp('MyWebApp', 'staging')
                }
            }
        }
    }
}