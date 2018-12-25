pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        git(url: 'https://github.com/antonovr/kafka-connect-hbase.git', branch: 'test-jenkins-blue-ocean', poll: true)
      }
    }
    stage('') {
      steps {
        withMaven(globalMavenSettingsConfig: '511bfa0a-f6bc-4a8d-9cba-4fb1a6bedff3', maven: 'M3', mavenLocalRepo: '.repository') {
          sh 'mvn clean install'
        }

      }
    }
  }
}