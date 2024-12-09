pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './grade build --no-deamon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}