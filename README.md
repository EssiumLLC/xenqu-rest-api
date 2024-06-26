# Essium's Xenqu Platform API

This repo holds supporting images and files for configuring a Postman environment and globals so you can begin testing.

View the docs at https://apidocs.xenqu.com/

To use the API you'll need:

* Client ID and Secret
* Public/Private 2048-bit RSA Self-Signed SSL keypair in PEM format
* A Xenqu subscriber account you want to access

You provide the cert (we need the public key, you keep the private key safe) and we provide the rest.  Here's the openssl command to generate your certificate:

    openssl req -newkey rsa:2048 -nodes -keyout privatekey.pem -x509 -out publickey.pem

Need more information on setting up a Xenqu account?  Head on over to https://essiumlabs.com to learn more and contact sales.

## Other Implementations

#### Ruby
We've open sourced our Ruby implementation of our API which can serve as a good reference for other implementation if you don't use Ruby.

https://github.com/EssiumLLC/lib-xenqu-ruby

#### .NET
We also started a .NET implementation which can access reports.  We've used this in RPA projects using Automation Anywhere.  It should also be possible to get it to work with UiPath.  Or it can used stand-alone to build utility apps.

https://github.com/EssiumLLC/lib-xenqu-dotnet

#### NodeJS (with TypeScript support)
We have also written a NodeJS implementation of our API

https://github.com/EssiumLLC/lib-xenqu-nodejs
