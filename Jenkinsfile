pipeline 
 {
  agent any
  stages 
   { 
    stage('Build')
     {
      steps
       {
        echo 'Building...'
        sh "composer install"
       }
     }
    stage('Test')
     {
      steps 
       {
        echo 'Testing...'
        sh "vendor/bin/phpunit -c module/Application/tests"
       }
     }
    stage('Deploy')
     {
      steps
       {
        echo 'Deploying...'
       }
     }
   }
 }
