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
    when {
      anyof {
       branch 'main'
       tag "*"
       }
    }
    steps{
      echo 'code Quality'
      }
    }

    stage('Unit Tests'){
    when {
          anyof {
           branch 'main'
           tag "*"
           }
        }
     steps{
       echo 'code Quality'
       }
     }

    stage('Download Dependencies') {
     when { tag "*" }
      steps {
        echo 'Download Dependenciess'
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
