pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                javac HelloWorld.java
            }
        }
        stage('Run') {
            steps {
                java HelloWorld
            }
        }
    }
}
