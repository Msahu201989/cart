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
    when { branch 'main' }
       steps {
         echo 'code Quality'

       }
      }

      stage('Unit Test') {
      when { branch 'main' }
          steps {
            echo 'code Quality'

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
