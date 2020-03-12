node('master') 
{
    stage('ContinuousDownload_master')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_master')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_master')
    {
        sh 'echo "deployed successfully"'
    }
    
    
    
    
}
