# curl-function

OpenFaaS curl in a Docker image

## Instructions

This image can be deployed to OpenFaaS in order to test service connectivity with `curl`.

```
git clone https://github.com/alexellis/curl-function
cd curl-function

faas-cli deploy

echo -n "-s http://gateway.openfaas:8080/system/info" | faas-cli invoke curl

echo -n "-s http://admin:password@gateway.openfaas:8080/system/info" | faas-cli invoke curl
```

Requirements: OpenFaaS and faas-cli.


