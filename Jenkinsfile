pipeline 
{
agent any
    stages
    {
      stage('S3download') 
        {      
            steps {
                withAWS(region:' us-east-1',credentials:'mykeys')\
                {
                    s3Download(file: 'apache-tomcat-9.0.46.tar.gz', bucket: 'mdm-npss', path: 's3://mdm-npss/dev/')
                }
            }
        }
    }
}