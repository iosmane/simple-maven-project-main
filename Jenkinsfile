pipeline {
  agent {
    node {
      label 'win-agent'
    }

  }
  stages {
    stage('Clean') {
      steps {
        bat 'cd simple-maven-project-main && mvn -DskipTests clean'
      }
    }

    stage('Compile') {
      steps {
        bat 'cd simple-maven-project-main && mvn -DskipTests compile'
      }
    }

  }
}