pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        git(url: 'https://github.com/antonovr/kafka-connect-hbase.git', branch: 'test-jenkins-blue-ocean', poll: true)
      }
    }
  }
}