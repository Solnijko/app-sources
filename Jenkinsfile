pipeline {
  agent any
  stages {
    stage("Build") {
      steps {
        git url: 'https://github.com/Solnijko/application-sources.git'
        withMaven {
          sh "./mvnw spring-boot:build-image"
        }
      }
    }
  }
}
