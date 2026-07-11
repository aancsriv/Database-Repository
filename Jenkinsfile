pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Repository checked out successfully'
            }
        }

        stage('Execute SQL') {
            steps {
              bat 'sqlcmd -S AANCHAL\\SQLEXPRESS -U jenkinsuser -P Jenkins@123 -d PracticeDB -i scripts\\001_CreateEmployee.sql'
            }
        }
    }
}