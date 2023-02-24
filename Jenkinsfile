pipeline {
    agent {
        node {
            label 'master'
        }
    }
    stages {
        stage('Inits') {
            steps {
                echo $JAVA_HOME
                which java
                which javac
            }
        }
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