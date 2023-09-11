pipeline {
  agent { label 'php' }
  
  stages {
    stage('PHP Version') {
      steps {
        sh 'php -v'
      }
    }
    stage('Test PHPUnit') {
      steps {
        sh 'phpunit --version'
      }
    }
    stage('Run PHPUnit Tests') {
      steps {
        sh 'phpunit --bootstrap src/autoload.php tests'
      }
    }
  }
}
