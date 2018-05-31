node
{
  stage('checkout')
  {
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/ssairram/firstrepo.git']]])
    properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('H/15 * * * *')])]) 
  }
   stage('build')
   {
    echo "build the code"
   }
   stage('test')
   {
    echo "test the build"
   }
   stage('delivery')
   {
    echo "deliver the code"
   }
}
