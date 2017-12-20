node('master') {
  
   stage 'Git Checkout'
     git 'https://github.com/venkatesh1993/spring-petclinic.git'
         echo 'checkout done'

   stage('Maven Build'){
      echo 'Maven Project Build'
      maven 'clean install'
      } 
      post {
          success {
              junit 'target/surefire-reports/**/*.xml' 
           }
      }
   }


   stage 'Test Case'
        echo 'Test Case will running'

   stage 'Reporting'
        echo 'Reporting Getting Creating'

   stage 'Job Status Status'
        echo 'Notification Sending'
}
