{
  agent any
  tools {
    nodejs 'NodeJS-20.x'  // Matches the Global Tool Configuration name
  }
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'  // Assumes `test` script exists in package.json
      }
    }
    stage('Build') {
      steps {
        sh 'npm run build'  // For React/Next.js apps
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploying to staging..."'
        // Add deployment commands (e.g., SSH, AWS S3, Docker)
      }
    }
  }
}

