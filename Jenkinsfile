pipeline {
  agent any
  parameters {
    string(name: 'STATEMENT', defaultValue: 'df -h ;pwd', description: 'What should I say?')
  }
  stages {
    stage('Example') {
      steps {
        /* CORRECT */
        sh '"${STATEMENT}"'
      }
    }
  }
}
