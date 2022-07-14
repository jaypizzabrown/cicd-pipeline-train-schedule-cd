pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon --stacktrace --debug --info'  
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        
        stage('Build2') {
            steps {
                echo 'Running build automation 2 '
            }
        }
    }
}
