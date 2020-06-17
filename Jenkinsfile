#!/usr/bin/env groovy
pipeline {
  agent any

  stages {
    stage("Build") {
      steps {
        def mvn_version = 'M3'
withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ) {
  //sh "mvn clean package"
}
        sh 'mvn -v'
      }
    }
     stage("Buildn") {
      steps {
        sh 'mvn clean intsall'
      }
     }
    stage("Deploy") {
      steps {
        echo "Deploy!"
      }
    }
  }
}
