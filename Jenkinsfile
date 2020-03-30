node('master') 
{
    stage('ContinuousDownload_feature3')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_feature3')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_feature3')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
