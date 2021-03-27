pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                echo 'make' 
                echo "${env.BRANCH_NAME}"
                echo "${currentBuild.timeInMillis}"
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
                echo "${env.BUILD_NUMBER}"
                echo "time took to complete pipeline is ${currentBuild.duration}"
            }
        }
    }
}
