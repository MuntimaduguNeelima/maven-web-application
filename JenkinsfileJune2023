node{
 echo "Jenkins Home directory is : ${env.JENKINS_HOME}"
  echo "Jenkins Job name is : ${env.JOB_NAME}"
   echo "Jenkins build number is : ${env.BUILD_NUMBER}"
   
   properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '5', numToKeepStr: '5')), [$class: 'RebuildSettings', autoRebuild: false, rebuildDisabled: false], [$class: 'JobLocalConfiguration', changeReasonComment: ''], pipelineTriggers([pollSCM('* * * * *')])])
}
