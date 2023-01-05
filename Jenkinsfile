pipeline {
  agent any
  stages{ 
    stage('build'){
      steps{
        echo 'build'
      }
    }
    stage('test'){
      steps{
        sh 'pip install requirements.txt'
        sh 'python app.py'
      }
    }
    stage('deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
}
