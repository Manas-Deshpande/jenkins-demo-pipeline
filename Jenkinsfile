pipeline {
    agent any

   stage('Clone Code') {
    steps {
        git branch: 'main',
            url: 'https://github.com/Manas-Deshpande/jenkins-demo-pipeline.git'
    }
}

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Test') {
            steps {
                sh 'pytest'
            }
        }

        stage('Build Completed') {
            steps {
                echo 'Application Build Successful'
            }
        }
    }
}