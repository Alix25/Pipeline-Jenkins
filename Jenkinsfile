pipeline {
  agent any
  stages{ 
    stage('build'){
      steps{
        agent{
          docker { image 'python:3' }
        }
        echo 'build'
      }
    }
    stage('test'){
      steps{
        sh 'pip install -r requirements.txt'
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
