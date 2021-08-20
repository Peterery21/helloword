pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                git "https://github.com/Peterery21/helloword.git"
            }
        }
        stage('build') {
            steps {
                //
                sh '''
                cd src/main/java/
                javac com/company/helloword/Main.java
                '''
            }
        }
        stage('run') {
            steps {
                //
                sh '''
                cd src/main/java/
                java com/company/helloword/Main
                 '''
            }
        }
    }
}
