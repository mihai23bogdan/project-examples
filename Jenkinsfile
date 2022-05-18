pipeline {
    agent any
    stages {
      stage('Git Clone') {
        steps{
          git url:'https://github.com/mihai23bogdan/project-examples.git', branch: 'master'
        }
    }    
      stage ('compile') {
          steps {
              sh "mvn compile"
          }
      }
     stage ('deploy') {
          steps {
              sh " mvn deploy -e"
          }
      }
    }  
}  
