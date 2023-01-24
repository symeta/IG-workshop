# jar related linux cmd

```sh
# to check package name within a Jar file
jar -tvf <jar file name> |grep <package name>

# to download jar file package through PIP
pip install <jar file name, i.e. sagemaker-feature-store-pyspark-3.1>

# to download jar files and upload to s3 bucket
mkdir <dir name>/
cd <dir name>/
wget <jar file url>
tar -xvzf <jar tar file>
cd <specific jar dir>
aws s3 sync ./ <s3 bucket uri, i.e. s3://xxx/>

# to copy local files to s3 bucket
# one file from local disk to s3 bucket, take .jar file for instance
aws s3 cp xxx.jar s3://xxx/xxx.jar

# files under a dir to s3 bucket
aws s3 cp d:/data s3://<bucket name>/raw --recursive

# to copy s3 object to local disk
# take a .pem file for instance
aws s3 cp s3://xxx/xxx.pem /xxx/xxx/xxx.pem


```
