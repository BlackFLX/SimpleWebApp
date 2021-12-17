pipeline {
    agent any

    stages {
      stage('BuildImage') {
          steps {
              echo 'Build Dockerimage'
              sh 'docker build . -t simplewebapp:${BUILD_NUMBER}'
              sh 'docker save -o simplewebapp.tar simplewebapp:${BUILD_NUMBER}'
              archiveArtifacts artifacts: 'simplewebapp.tar', followSymlinks: false
          }
      }
    }
}
