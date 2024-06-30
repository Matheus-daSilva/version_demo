pipeline {
    agent none
    stages {
        stage('Build') {
            agent any
            steps {
                bat 'echo começando o build...'
                bat 'python -m py_compile hello.py'
                stash(name: 'compiled--results', includes: '*.py')
            }
        }
    }
}