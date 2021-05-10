#!/usr/bin/env groovy
line1
line2
<<<<<<< HEAD
line3
=======
>>>>>>> parent of 05ba14f... third line
pipeline {
  
 tools {
        maven 'Maven 3.6.3'
    
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

