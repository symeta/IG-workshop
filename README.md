# IG workshop

## to check package name within a Jar file
```sh
jar -tvf <jar file name> |grep <package name>
```

## to decompile jar file through IDEA

## to download jar file package through PIP
```py
pip install <jar file name, i.e. sagemaker-feature-store-pyspark-3.1>

#show install dir of the package
pip show <jar file name>
```
## to download jar files and upload to s3 bucket
```sh
mkdir <dir name>/
cd <dir name>/
wget <jar file url>
tar -xvzf <jar tar file>
cd <specific jar dir>
aws s3 sync ./ <s3 bucket uri, i.e. s3://xxx/>
