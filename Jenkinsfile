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
        sh "cd /var/lib/jenkins/workspace/DevOpsTest;/usr/local/bin/apache-maven-3.5.0/bin/mvn package"
      }
    }
  }
}
