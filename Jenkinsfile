Pipeline{
  node amazon-slave
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
