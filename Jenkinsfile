node{
  stage('Checkout sourcecode') {
    git branch: 'master', url: 'https://github.com/vijayan663/TestApp.git'
  }
  stage('Api Management'){
    apiManagement "ApiManagementRC.json"
  }
}
