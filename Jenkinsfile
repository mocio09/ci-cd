pipeline {
  agent any

  stages {
    stage('Print Message') {
      steps {
        echo 'Pipeline triggered by push event'
      }
    }

    stage('Additional Step on Merge') {
      when {
        branch 'main'
      }
      steps {
        echo 'Additional step executed on merge to master'
      }
    }
  }
}