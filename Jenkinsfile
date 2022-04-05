pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        sh 'echo "Hello World from stageONE"'
      }
    }

    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            sh 'echo "This is Stage2 from Parallel block"'
          }
        }

        stage('Parallel_01') {
          steps {
            sh 'echo "Parallel stage01"'
          }
        }

        stage('Parallel_02') {
          steps {
            sh 'echo "parallel stage 02"'
          }
        }

      }
    }

    stage('stage3') {
      steps {
        sh 'echo "This is in Parallel block"'
      }
    }

  }
}