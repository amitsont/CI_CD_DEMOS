pipeline {
  agent any
  parameters {
    string(name: 'STATEMENT', defaultValue: 'ls -ltr; date;uname -a;pwd', description: 'What should I say?')
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
