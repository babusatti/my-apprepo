pipeline {
    agent any
node{
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
