pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "hello word ! "
            }
        }

        
    }
    triggers {
    pollSCM('* * * * *')
}
}
