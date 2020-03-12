node('master') 
{
    stage('ContinuousDownload_feature-2')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_feature-2')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_feature-2')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
