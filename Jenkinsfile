node('master') {
  checkout([$class: 'GitSCM', branches: [[name: '*/master']], browser: [$class: 'GithubWeb', repoUrl: 'https://github.com/arghya1990/jenkinsPipelineBuildTestDeploy'], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/arghya1990/jenkinsPipelineBuildTestDeploy.git']]])
  bat 'mvnw.cmd clean install'
  bat '''cd dockerdocker build -t spring-petclinic .'''docker build -t spring-petclinic .'''
  
  
  
  
}
