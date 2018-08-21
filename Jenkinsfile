pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'hugo'
      }
    }
    stage('Deploy') {
      steps {
        sh 'rsync -av ./public/ pockost-docker0:/srv/pockost_website_var_www_html/demo/'
      }
    }
  }
}
