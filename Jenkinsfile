pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building HTML Application'
            }
        }

        stage('Validate') {
            steps {
                sh '''
                if [ ! -f index.html ]; then
                    echo "index.html not found"
                    exit 1
                fi
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application'
            }
        }
    }
}
