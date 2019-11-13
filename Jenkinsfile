pipeline {
   agent any

   stages {
      stage('clone') {
         steps {
            bat 'git clone https://github.com/cwpang2000/training.git'
            bat 'chmod 777 '
            bat 'cd training'
            
         }
      }
      stage('build') {
         steps {
            echo 'this is build'
            bat ' javac App.java '
         }
      }
      stage('run') {
         steps {
            echo 'this is run'
            bat 'java App.class'
         }
      }
   }
}
