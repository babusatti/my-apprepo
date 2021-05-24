#!/usr/bin/env groovy
pipeline {
  
 tools {
        maven 'maven2'
    
    }
 
 
  agent any

  stages {
    stage("CheckOut-SCM") {
      steps {
        sh "git 'https://github.com/babusatti/my-apprepo.git'"
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

