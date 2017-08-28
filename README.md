# OpenSSL CA Helpers

This repo contains a set of scripts to simplify the creation of a self signed PKI using OpenSSL.

If your doing this at large scale please look at LetsEncrypt before considering to use this project.

If you are not familiar with PKI please read up on the various types of keys and certificates to avoid misconceptions
about the grantees it will provide as well as precautions you must take to keep keys protected.

## Helper Scripts:

- `createRoot` - Creates a root key which will be used in issuance of intermediate CAs.
- `createInterCA <purpose>` - Creates an intermediate CA which can be used for the given purpose.
- `createUserCA <Inter_CA_Dir> <User-Or-Domain-Naem>` - Creates a user cert with a signing chain.

These scripts are designed to provide a framework that you can extend for your own purposes, say a VPN or internal
authentication schemes.

## References:

## License:

MIT...

