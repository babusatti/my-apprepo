#!/usr/bin/env groovy
pipeline {
  agent any

  stages {
    stage("Build") {
      steps {
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
