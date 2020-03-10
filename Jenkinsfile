node('master') 
{
    stage('ContinuousDownload_master')
    {
       git 'https://github.com/ravi282/multibranch.git'
    } 
    stage('ContinuousBuild_master')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_master')
    {
        sh 'scp /var/lib/jenkins/workspace/multibranch_loan/webapp/target/webapp.war ubuntu@172.31.45.23:/home/ubuntu/var/lib/tomcat8/webapps/qaenv.war'
    }
    
    
    
    
}
