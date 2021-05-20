pilpelineP{
  agent any
  tools{
    maven 'M2_HOME'
  }
  stages {
    stage('Build'){
      step {
        sh 'mvn clean'
        sh 'install'
        sh 'mvn package'
      }
    }
     stage('test'){
      step {
        sh 'mvn test'
      }
    }
     stage('deploy'){
      step {
        echo "deploy step"
        sleep 10
      }
    }
     stage('docker'){
      step {
        echo "image step"
        sleep 10
      }
    }
  }
}
