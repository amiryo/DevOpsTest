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
        sh 'cd spring-boot-package-war;/usr/local/bin/apache-maven-3.5.0/bin/mvn package'
      }
    }
    stage('Test') {
      steps {
        sh 'cd spring-boot-package-war;/usr/local/bin/apache-maven-3.5.0/bin/mvn test'
      }
    }
  }
}