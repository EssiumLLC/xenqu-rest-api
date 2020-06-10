# Essium's Xenqu Platform API

This repo holds supporting images and files for configuring a Postman environment and globals so you can begin testing.

View the docs at https://apidocs.xenqu.com/

To use the API you'll need:

* Client ID and Secret
* Public/Private 2048-bit RSA Self-Signed SSL keypair in PEM format
* A Xenqu subscriber account you want to access

You provide the cert (we need the public key, you keep the private key safe) and we provide the rest.  Here's the openssl command to generate your certificate:

    openssl req -newkey rsa:2048 -nodes -keyout privatekey.pem -x509 -out publickey.pem

Need more information on setting up a Xenqu account?  Head on over to https://essium.co to learn more and contact sales.
