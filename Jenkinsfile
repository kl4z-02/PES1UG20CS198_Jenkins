pipeline{
    agent any
  stages{
    stage('Build'){
      steps{
          sh 'make -C main'
          echo 'Build success'
      }
    }
    stage('Test'){
      steps{
        sh 'STUFF I ADDED TO MAKE ERROR'
        sh '/var/jenkins_home/workspace/PES1UG20CS198-1/main/hello_exec'
        sh '/var/jenkins_home/workspace/PES1UG20CS198-1/main/working'
        echo 'Test success'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deployment success'
      }
    }
  }
    post{
      failure{
        echo 'Pipeline failed'
      }
    }
  }

