pipeline {
  agent any
  environment {
  dockerHome = "tool 'DockerInstallation'"
  mavenHome = "tool 'MavenInstallation'"
  }

  stages {
  stage('Build') {
    steps {
      // One or more steps need to be included within the steps block.
      echo "Build Stage"
      echo "PATH - $PATH"
      echo "JOB_NAME - $env.JOB_NAME"

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
