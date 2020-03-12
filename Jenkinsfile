node('master') 
{
    stage('ContinuousDownload_feature')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_feature')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_feature')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
