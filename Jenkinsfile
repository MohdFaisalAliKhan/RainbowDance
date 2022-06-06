pipeline {
    agent any
    environment{
        NAME="Faisal"
    }

    stages {
        stage('Build') {
            steps {
                echo "Building..for ${NAME}"
            }
        }
        stage('Test') {
            when{
                expression{
                    env.BRANCH_NAME=='dance'
                }
            }
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
