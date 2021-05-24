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
        git 'https://github.com/babusatti/my-apprepo.git'
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

