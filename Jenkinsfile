pipeline {
  agent any
  stages {
    stage('CloneGit') {
      steps {
        git(url: 'https://github.com/amiryo/DevOpsTest.git', branch: 'master')
      }
   } 
    stage('Build') {
      steps {
        sh "mvn package"
      }
    }
  }
}
