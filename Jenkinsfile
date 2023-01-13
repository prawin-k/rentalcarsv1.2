node(){
  stage("Git chekout"){
    checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'gitcreds', url: 'https://github.com/muraliphani/rentalcarsv1.2.git']])
  }
  stage("Maven Build"){
  sh "mvn package"
  }
}