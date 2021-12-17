pipeline {
    agent any

    stages {
      stage('Build') {
          agent {
              docker {
                  image 'python:latest'
              }
          }
          steps {
              echo 'Building'
          }
      }
      stage('BuildImage') {
          agent {
              docker {
                  image 'python:latest'
              }
          }
          steps {
              echo 'Build Dockerimage'
          }
      }
    }
}
