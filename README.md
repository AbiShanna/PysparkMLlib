# PysparkMLlib
**ML pipeline for sentiment classification**
<br/><br/>
**S3(input data) --> ML Pipeline (Tokenizer, StopWordsRemover, Hasing, Encoding)--> Classification model --> output sentiment predictions --> S3 bucket**
<br/>
S3 connection configuration:<br/>
_    
    hadoop_conf = spark._jsc.hadoopConfiguration() <br/>
    hadoop_conf.set("fs.s3n.impl", "org.apache.hadoop.fs.s3native.NativeS3FileSystem")<br/>
    hadoop_conf.set("fs.s3n.awsAccessKeyId", '************') <br/>
    hadoop_conf.set("fs.s3n.awsSecretAccessKey", '******************************') <br/>

_<br/>
Sample execution output :
<br/><br/>
![alt text](./output.PNG)<br/>

