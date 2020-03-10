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
        sh 'scp /var/lib/jenkins/workspace/multibranch1/webapp/target/webapp.war ubuntu@172.31.39.139:/home/ubuntu/var/lib/tomcat8/webapps/qaenv.war'
    }
    
    
    
    
}
