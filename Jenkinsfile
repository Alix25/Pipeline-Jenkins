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
        sh 'pip install -r requirements.txt'
        sh 'FLASK_APP=app.py flask run'
      }
    }
    stage('deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
}
