pipeline {
  agent any
  stages {
    stage('CloneGit') {
      steps {
        git(url: 'https://github.com/amiryo/DevOpsTest.git', branch: 'master')
    stage('CloneGit') {
      steps {
        sh "mvn package"
         }
       }
     }
    }
  }
}
