---
title: docker/ucp images
description: Verify the UCP images on this node
keywords: ucp, cli, images
---

Verify the UCP images on this node

## Usage

```
docker container run --rm -it \
        --name ucp \
        -v /var/run/docker.sock:/var/run/docker.sock \
        docker/ucp \
        images [command options]
```

## Description

This command checks the UCP images that are available in this node, and pulls
the ones that are missing.


## Options

| Option                        | Description                                          |
|:------------------------------|:-----------------------------------------------------|
| `--debug, D`                  | Enable debug mode                                    |
| `--jsonlog`                   | Produce json formatted output for easier parsing     |
| `--list`                      | List all images used by UCP but don't pull them      |
| `--pull` *value*              | Pull UCP images: `always`, when `missing`, or `never`|
| `--registry-password` *value* | Password to use when pulling images                  |
| `--registry-username` *value* | Username to use when pulling images                  |
