pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'The Running build automation'
                echo 'The Running2 build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
