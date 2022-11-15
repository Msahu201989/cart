pipeline {

 agent any

 stages {

  stage('code Quality') {
   steps{
     echo 'code Quality'
     sh 'env'
     }
   }

   stage('Style Checks') {
    steps{
      echo 'code Quality'
      }
    }

    stage('Unit Tests'){
     steps{
       echo 'code Quality'
       }
     }

    stage('Download Dependencies') {
     when { tag "*" }
      steps {
        echo 'Download Dependencies'
        }
        }

    stage('Prepare Artifact') {
      when { tag "*" }
      steps {
        echo 'Prepare Artifact'
        }
        }

    stage('Publish Artifact') {
      when { tag "*" }
      steps {
        echo 'Publish Artifact'
        }
        }
    }
 }
