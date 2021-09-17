pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        // Conditions
        // Only define expression of either Build Status or Build Status Change
            // Build Status Change :- if last build status change to green
        always {
            // This logic always executed, even the build succeeded or not.
            // e.g, sending the email to the team about the build condition.
        }
        success {
            // This logic only executed, when build succeeded
        }
        failure {
            // This logic only executed, when build failed
        }
    }
}
