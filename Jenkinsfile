pipeline {
    agent any

    stages {
      stage('BuildImage') {
          steps {
              echo 'Build Dockerimage'
              sh 'docker build . -t localhost:5000/simplewebapp:${BUILD_NUMBER}'
              sh 'docker image push http://localhost:5000:simplewebapp:${BUILD_NUMBER}'
          }
      }
    }
}
