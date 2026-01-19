pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/gjayavarshini8/html.git'
            }
        }

        stage('Deploy to Nginx') {
            steps {
                bat '''
                xcopy /E /Y /I womenclothing\* C:\nginx\nginx-1.28.1\html
                '''
            }
        }
    }
}
