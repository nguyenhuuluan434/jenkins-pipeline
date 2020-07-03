pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Get source') {
      steps {
        git(url: 'https://github.com/nguyenhuuluan434/jpa-specification', branch: 'master', poll: true, changelog: true)
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