pipeline {
    agent any
    stages{
    stage('init'){
      //init sample
    }
    stage('build'){
        withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
    }
    
}
}
