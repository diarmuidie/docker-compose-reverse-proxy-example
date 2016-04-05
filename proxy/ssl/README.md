The following commands can be used to generate a self signed ssl key and certificate

To generate the key:

```sh
openssl genrsa -out microservice1-test.key 2048
```

And the certificate (replace `microservice1.test` with your domain name):

```sh
openssl req -new -x509 -key microservice1-test.key -out microservice1-test.cert -days 3650 -subj /CN=sample-microservice1.test
```
