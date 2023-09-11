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
        sh './vendor/bin/phpunit --version'
      }
    }
    stage('Run PHPUnit Tests') {
      steps {
        sh './vendor/bin/phpunit tests'
      }
    }
    stage('Run PHPUnit TestDox Tests') {
        sh './vendor/bin/phpunit --testdox tests'
    }
  }
}
