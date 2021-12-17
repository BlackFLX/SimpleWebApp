pipeline {
    agent any

    stages {
      stage('BuildImage') {
          steps {
              echo 'Build Dockerimage'
              sh 'docker build . -t simplewebapp:${BUILD_NUMBER}'
          }
      }
    }
}
