pipeline {
  agent any
  parameters {
    string(name: 'STATEMENT', defaultValue: 'pwd', description: 'What should I say?')
  }
  stages {
    stage('Example') {
      steps {
        /* CORRECT */
        sh "${STATEMENT}"
      }
    }
  }
}
