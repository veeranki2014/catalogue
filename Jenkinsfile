pipeline {
  agent {
    node { label 'workstation'}
  }

  stages {
    stage ('Build code') {
      steps {
        sh 'npm install'
      }
    }

    stage ('Unit Testing') {
          steps {
            echo "Unit Testing"
          }
    }


    stage ('Code Analysis') {
          steps {
            echo "Code Analysis"
            //sh 'sudo sonar-scanner -Dsonar.host.url=http://172.31.88.214:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=catalogue'
          }
    }

    stage ('Security checks') {
          steps {
            echo "Security checks"
          }
    }

    stage ('Code Publish') {
          steps {
            echo "Code Publish"
          }
    }
  }

//   post {
//     always {
//
//     }
//   }



}