@Library("mylibs") _
pipeline {
  /*agent any
  tools {
    maven 'maven2'
  } */
  stages{
     stage("git checkout"){
      steps{
        checkout scmGit(branches: [[name: '*/mastert']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/GRR1317/my-app.git']])
      }
    }
  /*  stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
      stage("Deploy To Dev"){
      steps{
        tomcatDeploy("tomcat-dev","ec2-user",["172.31.13.89","172.31.13.89"])
      }
    }  */
  }
}
