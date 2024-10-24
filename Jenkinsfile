pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
              echo 'running build'
              sh './gradlew build --no-daemon'
              archiveArtifacts artifacts: 'dist/trainSchedule.zip'
              
                
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
}
