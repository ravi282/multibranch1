node('loan') 
{
    stage('ContinuousDownload_loan')
    {
       git 'https://github.com/ravi282/multibranch.git'
    } 
    stage('ContinuousBuild_loan')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_loan')
    {
        sh 'scp /var/lib/jenkins/workspace/multibranch_loan/webapp/target/webapp.war root@172.31.45.23:/var/lib/tomcat8/webapps/qaenv.war'
    }
    
    
    
    
}
