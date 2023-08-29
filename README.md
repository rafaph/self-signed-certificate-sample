# Self signed certificate sample

The idea of this project is to be a sample of using docker compose to create a service and access it through https.

## Requirements

- [docker](https://docs.docker.com/get-docker/)
- [just](https://github.com/casey/just)

## Usage

### Start

```
just up
```

This will generate the file `certs/ca.crt` among others.

### Install certificate

Install the certificate on your preferred browser, [more details here](https://github.com/sebastienheyd/docker-self-signed-proxy-companion#trust-self-signed-certificates).

> Note: For Chrome, choose to import on the `Trusted Root Certification Authorities tab`.

### Restart your browser

After restarting your browser, access `https://nginx.localtest.me` and see what magic happens.
