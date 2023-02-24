pipeline {
    agent {
        node {
            label 'master'
        }
    }
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
