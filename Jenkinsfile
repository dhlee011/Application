pipeline {
  agent any
  stages {
    stage('git scm update') {
      steps {
        git url: 'https://github.com/dhlee011/Gitops_Test.git', branch: 'main'
      }
    }
    stage('dockerfile build ') {
      steps {
        app = docker.build("902268280034.dkr.ecr.ap-northeast-2.amazonaws.com/test-ecr")
      }
    }

  }
}
