pipeline {
    agent any
    stages {
      stage('Git Clone') {
        steps{
          git url:'https://github.com/mihai23bogdan/project-examples/tree/master/maven-examples/maven-example', branch: 'master'
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
