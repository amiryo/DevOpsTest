pipeline {
  agent {
    node {
      label 'Pipe1'
    }
    
  }
  stages {
    stage('ImportGIT') {
      steps {
        git(url: 'https://github.com/amiryo/DevOpsTest.git', branch: 'master', changelog: true, poll: true)
      }
    }
  }
}