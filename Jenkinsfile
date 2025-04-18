pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // This forces a full checkout regardless of Jenkins config
                checkout scm
            }
        }
        stage('Print Commit Info') {
            steps {
                script {
                    def commitMessage = sh(script: 'git log -1 --pretty=%B', returnStdout: true).trim()
                    def commitHash = sh(script: 'git rev-parse HEAD', returnStdout: true).trim()
                    echo "📝 Commit Message: ${commitMessage}"
                    echo "🔑 Commit Hash: ${commitHash}"
                }
            }
        }
    }
}
