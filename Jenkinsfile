pipeline {
  agent any
  parameters {
    string(name: 'STATEMENT', defaultValue: 'hello; pwd', description: 'What should I say?')
  }
  stages {
    stage('Example') {
      steps {
        /* CORRECT */
        sh 'echo "${STATEMENT}"'
      }
    }
  }
}
