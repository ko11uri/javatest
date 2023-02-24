pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                script("javac HelloWorld.java")
            }
        }
        stage('Run') {
            steps {
                script("java HelloWorld")
            }
        }
    }
}
