pipeline {
  agent {
    node {
      label 'win-agent'
    }

  }
  stages {
    stage('Clean') {
      steps {
        bat 'mvn -B -DskipTests clean package'
      }
    }

    stage('Compile') {
      steps {
        bat 'mvn -B -DskipTests compile'
      }
    }

  }
}