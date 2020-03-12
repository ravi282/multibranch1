node('master') 
{
    stage('ContinuousDownload_feature2')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_feature2')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_feature2')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
