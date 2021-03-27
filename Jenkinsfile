pipeline{
  agent any
    stages{
         stage('1st')
        {
          steps {
            echo "Hello World"
                }
        }
      stage('2nd')
      {
        steps{
        checkout([$class: 'GitSCM', userRemoteConfigs: [url:https://github.com/amitsont/CI_CD_DEMOS]])
        }
      }
      }
}
