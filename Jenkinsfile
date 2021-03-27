pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                echo 'make' 
                echo "${withEnv.BRANCH_NAME}"
            }
        }
        stage('Test'){
            steps {
                echo 'make check'
                echo "${JOB_NAME}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'make publish'
            }
        }
    }
}
