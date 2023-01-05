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
        sh 'python -m unittest discover'
      }
    }
    stage('deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
}
