pipeline {
  agent any
  stages {
    stage('Get source') {
      parallel {
        stage('Get source') {
          steps {
            git(url: 'https://github.com/nguyenhuuluan434/jpa-specification', branch: 'master', poll: true, changelog: true)
          }
        }

        stage(' source 3rd') {
          steps {
            git(url: 'https://github.com/javaee-samples/javaee7-samples.git', branch: 'master')
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh '''#!/bin/bash
echo test'''
      }
    }

  }
  environment {
    a = 'a'
  }
}