pipeline{
  agent any
  tools {
        // Must match the Name in 'Global Tool Configuration'
        maven 'Maven-M3' 
    }
  stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
     stage('Build') {
            steps {
                sh 'mvn -B clean package -DskipTests'
            }
        }
    }
}
