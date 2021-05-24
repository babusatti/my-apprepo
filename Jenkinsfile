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
        sh 'git clone https://github.com/babusatti/my-apprepo.git'
            }
                   }
   
    
     stage("Build jar") {
      steps {
        sh 'mvn -f pom.xml clean install'
           }
                    }
    stage("Deploy") {
      steps {
        echo "Deploy!"
            }
                    }
          }
}

