pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo '===== Stage 1: Build ====='
                echo 'Task: Build the code using a build automation tool to compile and package the application.'
                echo 'Tool: Maven - A powerful build automation tool used primarily for Java projects. Maven compiles source code, resolves dependencies, and packages the application into deployable artifacts (e.g., JAR or WAR files).'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo '===== Stage 2: Unit and Integration Tests ====='
                echo 'Task: Run unit tests to ensure the code functions as expected and run integration tests to ensure the different components of the application work together as expected.'
                echo 'Tools:'
                echo '  - JUnit: A widely used testing framework for Java applications. It is used to write and execute unit tests to verify individual components of the code behave correctly in isolation.'
                echo '  - Selenium: An open-source framework used for automating web browser interactions. It is used here for integration testing to ensure various components of the application work together as expected in a browser environment.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo '===== Stage 3: Code Analysis ====='
                echo 'Task: Analyse the code using a code analysis tool to ensure it meets industry standards, identify code smells, and enforce coding best practices.'
                echo 'Tool: Checkstyle - A static code analysis tool for Java that enforces a coding standard. It examines source code against a defined set of rules covering code style, formatting, and potential issues, ensuring code quality and maintainability.'
            }
        }

        stage('Security Scan') {
            steps {
                echo '===== Stage 4: Security Scan ====='
                echo 'Task: Perform a security scan on the code to identify known vulnerabilities, exposure of sensitive data, and security misconfigurations.'
                echo 'Tool: OWASP Dependency-Check - An open-source Software Composition Analysis (SCA) tool that detects publicly disclosed vulnerabilities contained within project dependencies. It scans project libraries and reports them against the National Vulnerability Database (NVD) CVE list.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo '===== Stage 5: Deploy to Staging ====='
                echo 'Task: Deploy the compiled and tested application to a staging server that mirrors the production environment.'
                echo 'Tool: AWS CLI / AWS Elastic Beanstalk - The AWS Command Line Interface is used to automate deployment to an AWS EC2 instance or Elastic Beanstalk environment. The staging environment closely mirrors production, allowing safe pre-release validation without affecting end users.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo '===== Stage 6: Integration Tests on Staging ====='
                echo 'Task: Run integration tests on the staging environment to ensure the application functions as expected in a production-like environment, verifying end-to-end workflows and service interactions.'
                echo 'Tool: Selenium WebDriver - Used to run automated end-to-end integration tests against the deployed staging application. These tests simulate real user interactions in a browser to confirm the application behaves correctly in the staging environment before promotion to production.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo '===== Stage 7: Deploy to Production ====='
                echo 'Task: Deploy the fully tested and validated application to the production server, making it available to end users.'
                echo 'Tool: AWS CodeDeploy - An AWS deployment service that automates application deployments to Amazon EC2 instances. It ensures reliable, zero-downtime deployments to production by supporting rolling updates and blue/green deployment strategies, minimising disruption to end users.'
            }
        }

    }
}
