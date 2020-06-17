#!/usr/bin/env groovy
pipeline {
  
 tools {
        maven 'Maven 3.6.3'
        jdk 'jdk8'
    }
 
 
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

