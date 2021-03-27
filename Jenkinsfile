pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                echo 'make' 
                echo "${env.BRANCH_NAME}"
            }
        }
        stage('Test'){
            steps {
                echo 'make check'
                echo "${env.JOB_NAME}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'make publish'
            }
        }
    }
}
