pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Task: Compile and package the application code.'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests to verify individual components, and integration tests to verify components work together.'
                echo 'Tool: JUnit (unit), TestNG (integration)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse code quality and check it meets industry standards.'
                echo 'Tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Task: Scan the code/dependencies for known vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to a staging server for pre-production testing.'
                echo 'Tool: AWS EC2 (via Ansible)'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests against the staging environment to confirm production-like behaviour.'
                echo 'Tool: Postman/Newman'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the verified application to the production server.'
                echo 'Tool: AWS EC2 (via Ansible)'
            }
        }
    }
}
