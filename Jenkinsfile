pipeline {
  agent any

  
  stages {
    stage('shellcopy') {
      steps {
        script {
          try {
            sh(script: 'cp /var/local/go.conf /etc/nginx/', returnStdout: true)
          } catch (Exception ex) {
            echo 'Exception: ' + ex.toString()
          }
        }
      }
    }
