# Golang SSH KeyPair Generator with S3 Backup

Keygen generates AES256 private and public key pairs and uploads the private key to a desired S3 bucket.

## Usage

**Required packages:**

`go get github.com/aws/aws-sdk-go/aws`

`go get github.com/aws/aws-sdk-go/aws/session`

`go get github.com/aws/aws-sdk-go/service/s3`

`go get golang.org/x/crypto/ssh`

**Compile:**

**Windows:**  `GOOS=windows GOARCH=386 go build -o keypair_generator.exe keypair_generator.go`

**Linux:**    `GOOS=linux GOARCH=386 go build -o keypair_generator.exe keypair_generator.go`

**MacOS:**    `GOOS=darwin GOARCH=386 go build -o keypair_generator.exe keypair_generator.go`

# Important: 

## Set Authentication

`export AWS_DEFAULT_REGION=eu-west-2`

`export AWS_ACCESS_KEY_ID=ABCDEF`

`export AWS_ACCESS_SECRET_KEY=Zzxx`

## Set Target

`export S3_BUCKET=bucketname`

## Set Desired Key Name

`export PRIKEY=keyname`

`export PUBKEY=keyname.pub`
