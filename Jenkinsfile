pipeline {
  agent any
  tools {
     maven 'M2_HOME'
  }
    stages {
        stage('Build'){
            steps {
              sh 'mvn clean'
              sh 'mvn install'
              sh 'mvn package'
            }
        }
      stage('test'){
            steps {
             echo "test"
                sh ' mvn test'
            }
        }
      stage('deploy'){
            steps {
             echo "deploy step"
                sleep 10
            }
        }
      stage('docker'){
            steps {
             echo "docker image"
                sleep 10
            }
        }
    }
}
