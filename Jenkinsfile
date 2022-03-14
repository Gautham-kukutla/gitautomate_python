pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                sh'''rm -rf task
                git clone https://github.com/Gautham-kukutla/python.git task
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
                sh'''pip install GitPython
                cd task
                pwd
                git remote set-url origin https://Gautham-kukutla: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@github.com/Gautham-kukutla/python.git
                python3 python_script.py
                chmod +x script2.sh
                ./script2.sh
                '''

            }
        }
    }
}
