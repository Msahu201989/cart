//@Library('augustroboshop') _

//env.COMPONENT="cart"   //this is project key for Sonar
//nodejs()

pipeline {

 agent any

  stages {

   stage('codes Quality') {
    steps {
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
       steps {
         echo 'code Quality'

       }
      }

      stage('Unit Test') {
    when {
       anyof {
        branch 'main'
         tag "*"
       }
       }

     stage('Download Dependencies') {
      when { tag "*"}
        steps {
         echo 'Download Dependencies'

           }
           }


     stage('Prepare Artifacts') {
      when { tag "*"}
        steps {
         echo 'Prepare Artifacts'

           }
           }

        stage('Publish Artifacts') {
         when { tag "*"}
           steps {
            echo 'Publish Artifacts'

              }
              }

  }
}
