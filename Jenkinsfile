pipeline{
  agent any
  tools{
    maven "maven"
  }
  stages{
    stage('scm-checkout') {
      steps{
        git 'https://github.com/tirupathi-naidu/maven-web-application'
      }
    }
    stage('build') {
      steps{
        sh 'mvn package'
      }
    }
  }
}
