node('master') 
{
    stage('ContinuousDownload_release')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_release')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_release')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
