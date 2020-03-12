node('loan') 
{
    stage('ContinuousDownload_loan')
    {
       git 'https://github.com/ravi282/multibranch1.git'
    } 
    stage('ContinuousBuild_loan')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_loan')
    {
        sh 'echo "deployed loan branch"'
    }
    
    
    
    
}
