pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                echo 'make' 
                echo "${BRANCH_NAME}"
            }
        }
        stage('Test'){
            steps {
                echo 'make check'
                echo ${JOB_NAME}
            }
        }
        stage('Deploy') {
            steps {
                echo 'make publish'
            }
        }
    }
}
