node
{
  stage('checkout')
  {
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/ssairram/firstrepo.git']]])
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
