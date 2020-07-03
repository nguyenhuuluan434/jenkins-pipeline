pipeline {
  agent any
  stages {
    stage('Get source') {
      steps {
        git(url: 'https://github.com/nguyenhuuluan434/jpa-specification', branch: 'master', poll: true, changelog: true)
        build 'build'
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