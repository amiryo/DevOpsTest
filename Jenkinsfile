pipeline {
  agent any
  stages {
    stage('ImportGit') {
      steps {
        git(url: 'https://github.com/amiryo/DevOpsTest.git', branch: 'master')
      }
    }
  }
}