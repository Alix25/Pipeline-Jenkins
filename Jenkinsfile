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
        bat 'pip install -r requirements.txt'
        bat 'python app.py'
      }
    }
    stage('deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
}
