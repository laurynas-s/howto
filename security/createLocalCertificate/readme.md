* Create local test sertificate for HTTPS

```
> openssl genrsa 1024 > file.pem
> openssl req -new -key file.pem -out csr.pem
> openssl x509 -req -days 365 -in csr.pem -signkey file.pem -out file.crt
```
