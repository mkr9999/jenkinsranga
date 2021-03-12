pipeline {
  agent any
  environment {
  dockerHome = tool 'DockerInstallation'
  mavenHome = tool 'MavenInstallation'
  PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
  }

  stages {
  stage('Build') {
    steps {
      // One or more steps need to be included within the steps block.
      echo "Build Stage"
      echo "PATH - $PATH"
      echo "JOB_NAME - $env.JOB_NAME"
      sh 'mvn --version'
      sh 'docker --version'
    }
  }

  stage('Test') {
    steps {
      // One or more steps need to be included within the steps block.
      echo "Test Stage"
    }
  }
}
}
