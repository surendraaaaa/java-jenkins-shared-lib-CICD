@Library('my-shared-lib') _
pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                script {
                    gitcheckout(
                        branch: "main",
                        url: "https://github.com/surendraaaaa/java-jenkins-shared-lib-CICD.git"
                        )
                }
            }
        }

        stage('Unit test maven') {
            steps {
                script {
                    mvnTest()
                    
                }
            }
        }
    }
}

