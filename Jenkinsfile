@Library('my-shared-lib') _
pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                script {
                    gitcheckout(
                        branch: "shell_scripting",
                        url: "https://github.com/surendraaaaa/java-jenkins-shared-lib-CICD.git"
                        )
                }
            }
        }

        stage('Unit test maven') {
            steps {
                script {
                    mvmTest()
                    
                }
            }
        }
    }
}

