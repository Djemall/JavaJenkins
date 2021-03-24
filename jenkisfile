pipeline {
    agent any
    stages {
        stage('clone sources') {
            steps {
                git branch: 'main', url: 'https://github.com/Djemall/JavaJenkins.git'
            }
        }
        stage('build') {
            steps {
                sh "pwd"
                sh "javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "java Main"
            }
        }
    }
}
