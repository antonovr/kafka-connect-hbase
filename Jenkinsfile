pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        git(url: 'antonovr/kafka-connect-hbase', branch: 'master', poll: true)
      }
    }
  }
}