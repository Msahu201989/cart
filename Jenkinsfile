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
        when { tag "*" }
        steps {
         echo 'Download Dependencies'
        }
      }

       stage ('Prepare Artifact') {
        when { tag "*" }
         steps {
          echo 'Prepare Artifact'
         }
       }

         stage ('Publish Artifact') {
           when { tag "1.0.0" }
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
