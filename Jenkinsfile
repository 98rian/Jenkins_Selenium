pipeline {
    agent{label 'demoAgent'}

    stages {
        stage('git') {
            steps {
                git branch: 'master', url: 'https://github.com/98rian/Jenkins_Selenium.git'
            }
        }
        stage('mvn') {
            steps {
                bat 'mvn clean test'
            }
        }
    }
}
