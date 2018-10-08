# docker
A set of Dockerfiles for personal use. You may find them useful...or not.

## aws

The Amazon Web Services command line interface tool, `awscli`.

```
# Example: List files in an S3 bucket
$ docker run --rm -v -e AWS_ACCESS_KEY_ID=${AWS_ACCESS_KEY_ID} \
      -e AWS_SECRET_ACCESS_KEY=${AWS_SECRET_ACCESS_KEY} \
      -e AWS_DEFAULT_REGION=${AWS_DEFAULT_REGION} aws s3 ls s3://${S3_BUCKET}
```

## hugo

The [Hugo](https://gohugo.io) static site generator. Pass [Hugo commands](https://gohugo.io/commands/)
to the container to execute.

```
# Create a new site in the current directory on the host
$ docker run --rm --user $(id -u):$(id -u) -v $(pwd):/data hugo new site /data
```
