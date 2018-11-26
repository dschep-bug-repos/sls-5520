# https://github.com/serverless/serverless/issues/5520
```
$ git clone https://github.com/dschep-bug-repos/sls-5520
$ cd sls-5520
$ sls print
service: sls-5520
provider:
  name: aws
  runtime: nodejs8.10
functions:
  hello:
    handler: handler.hello
custom:
  bucket: sls-5520
  mode:
    dev: cloud
  externalConfigFromS3:
    foobar: |
      FOOBAR
```
