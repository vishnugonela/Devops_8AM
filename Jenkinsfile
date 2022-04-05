pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        sh 'echo "Hello World from stageONE"'
      }
    }
    stage('Stage2') {
      steps {
        sh 'echo "This is Stage2 from Parallel block"'
      }
    }
    stage('stage3'){
	steps{
	 sh 'echo "This is in Parallel block"'
	}


    }
  }
}
