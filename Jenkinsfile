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
                    def ar = ['one', 'two']
                    for (int i = 0; i < ar.size(); i++) {
                        sh("java HelloWorld ${ar[i]}")
                    }
                }
            }
        }
    }
}
