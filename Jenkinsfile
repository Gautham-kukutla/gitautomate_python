pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                bat'''rm -rf task
                git clone https://github.com/Gautham-kukutla/python.git task
                '''
            }
        }
        stage('Creating Files') {
            steps {
                bat '''cd task
                touch file.txt file1.txt file3.txt
                '''
            }
        }
        stage('Git Modification Check') {
            steps {
                bat'''pip install GitPython
                cd task
                pwd
                git remote set-url origin https://Gautham-kukutla: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@github.com/Gautham-kukutla/python.git
                python python_script.py
                chmod +x script2.sh
                bash script2.sh
                '''

            }
        }
    }
}
