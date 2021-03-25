pipeline {
  agent any
  stages {
    stage('Git-Checkout') {
      steps {
        git(url: 'https://github.com/rchidana/Accenture_Pipeline.git', branch: 'master')
        echo 'Git Checkout Successfull!!'
      }
    }

    stage('Compile') {
      steps {
        bat 'Compile.bat'
        echo 'Compiled Successfully!!'
      }
    }

    stage('Package') {
      steps {
        bat 'Package.bat'
        echo 'Package Successfully!!'
      }
    }

    stage('Deploy') {
      steps {
        bat 'Deploy.bat'
        echo 'Deployed SUccessfully!!'
      }
    }

  }
}