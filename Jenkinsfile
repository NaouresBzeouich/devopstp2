pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "hello word ! "
            }
        }

        stage('comit details') {
            steps {
                echo "🧬 Branch: ${env.GIT_BRANCH}"
                echo "🔁 Commit ID: ${env.GIT_COMMIT}"
                echo "📂 Repo: ${env.GIT_URL}"
                echo "🧑‍💻 Author Email: ${env.GIT_AUTHOR_EMAIL}"
                echo "🧑‍💻 Author Name: ${env.GIT_AUTHOR_NAME}"
                echo "📝 Commit Message: ${env.GIT_COMMIT_MESSAGE}"
            }
        }
    }
}
