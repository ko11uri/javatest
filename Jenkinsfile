pipeline {
    agent any

    stages {
        stage('Inits') {
            steps {
                echo $JAVA_HOME
                which java
                which javac
                env
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