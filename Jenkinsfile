pipeline {
  agent any
  stages {
    stage('CloneGit') {
      steps {
        git(url: 'https://github.com/amiryo/DevOpsTest.git', branch: 'master', changelog: true, poll: true)
      }
    }
    stage('Build') {
      steps {
        sh 'cd /var/lib/jenkins/workspace/DevOpsTest/spring-boot-package-war'
      }
    }
    stage('stam') {
      steps {
        sh 'ls -ltr'
      }
    }
    stage('error') {
      steps {
        cleanWs(cleanWhenFailure: true, cleanWhenNotBuilt: true)
      }
    }
  }
}