pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                sh'''rm -rf task
                git clone 'https://github.com/Gautham-kukutla/python.git' task
                '''
            }
        }
        stage('Creating Files') {
            steps {
                sh '''cd task
                touch file.txt file1.txt file3.txt
                '''
            }
        }
        stage('Git Modification Check') {
            steps {
                sh'''cd task
                pwd
                python3 python_script.py
                '''
            }
        }
    }
}
