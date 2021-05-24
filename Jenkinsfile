#!/usr/bin/env groovy
pipeline {
  
 tools {
        maven 'maven2'
    
    }
  
 
 
  agent any

  stages {
    
    stage("cleani ws") {
      steps {
        cleanWs()
            }
                   }
    
    stage("CheckOut-SCM") {
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

