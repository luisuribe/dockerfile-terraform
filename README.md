[![](https://badge.imagelayers.io/uzyexe/terraform:latest.svg)](https://imagelayers.io/?images=uzyexe/terraform:latest 'Get your own badge on imagelayers.io')

# uzyexe/terraform [![Circle CI](https://circleci.com/gh/uzyexe/dockerfile-terraform.svg?style=svg)](https://circleci.com/gh/uzyexe/dockerfile-terraform)

## What is terraform

Terraform provides a common configuration to launch infrastructure — from physical and virtual servers to email and DNS providers. Once launched, Terraform safely and efficiently changes infrastructure as the configuration is evolved.

Simple file based configuration gives you a single view of your entire infrastructure.

[https://www.terraform.io/](https://www.terraform.io/)

## Dockerfile

[**Trusted Build**](https://hub.docker.com/r/uzyexe/terraform/)

This Docker image is based on the official [alpine:3.4](https://hub.docker.com/_/alpine/) base image.

## How to use this image

```
docker run uzyexe/terraform [--version] [--help] <command> [<args>]

```

## Using

**Please note: Create by your Terraform configuration files (.tf) is `/data` directory**

### terraform apply

```
docker run --rm -it -v /data:/data uzyexe/terraform apply [options]
```

### terraform destroy

```
docker run --rm -it -v /data:/data uzyexe/terraform destroy [options] [DIR]
```

### terraform fmt

```
docker run --rm -it -v /data:/data uzyexe/terraform fmt [options] [DIR]
```

### terraform force-unlock

```
docker run --rm -it -v /data:/data uzyexe/terraform force-unlock LOCK_ID [DIR]
```

### terraform get

```
docker run --rm -it -v /data:/data uzyexe/terraform get [options] PATH
```

### terraform graph

```
docker run --rm -it -v /data:/data uzyexe/terraform graph [options]
```

### terraform import

```
docker run --rm -it -v /data:/data uzyexe/terraform [options] ADDR ID
```

### terraform init

```
docker run --rm -it -v /data:/data uzyexe/terraform init [options] SOURCE [PATH]
```

### terraform output

```
docker run --rm -it -v /data:/data uzyexe/terraform output [options] NAME
```

### terraform plan

```
docker run --rm -it -v /data:/data uzyexe/terraform plan [options]
```

### terraform providers

```
docker run --rm -it -v /data:/data uzyexe/terraform providers [config-path]
```

### terraform push

```
docker run --rm -it -v /data:/data uzyexe/terraform push [options]
```

### terraform refresh

```
docker run --rm -it -v /data:/data uzyexe/terraform refresh [options]
```

### terraform show

```
docker run --rm -it -v /data:/data uzyexe/terraform show terraform.tfstate [options]
```

### terraform state <subcommand> [options] [args]

```
docker run --rm -it -v /data:/data uzyexe/terraform state <subcommand> [options] [args]
```

### terraform taint

```
docker run --rm -it -v /data:/data uzyexe/terraform taint [options] name
```

### terraform untaint

```
docker run --rm -it -v /data:/data uzyexe/terraform untaint [options] name
```

### terraform validate

```
docker run --rm -it -v /data:/data uzyexe/terraform validate
```

### terraform version

```
docker run --rm -it uzyexe/terraform version
```

### terraform workspace

```
docker run --rm -it uzyexe/terraform workspace <subcommand> [options] [args]
```

# Authors

* Shuji Yamada (<uzy.exe@gmail.com>)

## License

This project is licensed under the terms of the MIT license.

