pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                sh('javac HelloWorld.java')
            }
        }
        stage('Run') {
            steps {
                script {
                    def ar = ['oneexample', 'twoexample',"three"]
                    for (int i = 0; i < ar.size(); i++) {
                        sh("java HelloWorld ${ar[i]}")
                    }
                }
            }
        }
    }
}
