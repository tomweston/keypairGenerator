# Golang SSH Key Generator with S3 Backup

Keygen generates AES256 private and public key pairs and uploads the keypair to a desired S3 bucket.

## Usage

You must first define the private and Public Key Names and AWS credentials by using the following environment variables:

## Set Authentication

`export AWS_DEFAULT_REGION=eu-west-2`

`export AWS_ACCESS_KEY_ID=ABCDEF`

`export AWS_ACCESS_SECRET_KEY=Zzxx`

## Set Target

`export S3_BUCKET=bucketname`

## Set desired Key Name

`export PRIKEY=keyname`

`export PUBKEY=keyname.pub`
