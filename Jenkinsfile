pipeline {

 agent any

 stages {

  stage ('code quality') {
    steps {
     echo 'code quality'
    }
  }

    stage ('Style checks') {
      steps {
       echo 'style checks'
      }
    }

      stage ('unit Tests') {
        steps {
         echo 'Unit Test'
        }
      }

      stage ('Download dependencies') {
        steps {
         echo 'Download Dependencies'
        }
      }

       stage ('Prepare Artifact') {
         steps {
          echo 'Prepare Artifact'
         }
       }

         stage ('Publish Artifact') {
           steps {
            echo 'Publish Artifact'
           }
         }
 }
 }










// @Library('roboshop') _
//
// env.COMPONENT="cart"
// nodejs()
