pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/gangarapu365/cicd.git'
      }
    }
    stage('Build') {
      steps {
        sh 'echo "✅ Build stage running..."'
      }
    }
    stage('Test') {
      steps {
        sh 'echo "✅ Test stage running (unit tests here)..."'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "✅ Deploying to /var/www/html (simulated)"'
        sh 'sudo cp index.html /var/www/html/index.html || true'
      }
    }
  }
}

