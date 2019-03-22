node{
  stage('Cleanup workspace') {
    step([$class: 'WsCleanup', deleteDirs: true, notFailBuild: true, patterns: [[pattern: '*', type: 'INCLUDE']]])
  }

  stage('Checkout sourcecode') {
    git branch: 'master', url: 'https://github.com/vijayan663/TestApp.git'
  }
  stage('Api Management'){
    apiManagement "ApiManagementRC.json"
  }
}
