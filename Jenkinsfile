#!/usr/bin/env groovy
pipeline {
  
 tools {
        maven 'maven2'
    
    }
 
 
  agent any

  stages {
    stage("Build") {
      steps {
        sh 'mvn -v'
            }
                   }
    
     stage("Build jar") {
      steps {
        sh 'mvn clean install'
           }
                    }
    stage("Deploy") {
      steps {
        echo "Deploy!"
            }
                    }
          }
}

