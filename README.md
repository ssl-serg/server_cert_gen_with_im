# server_cert_gen_with_im

Test server certificate generation script 

# Desc

It creates server certificate with CA and IM CA in chain: CA -> IM CA -> Server Cert

openssl.exe tool required to launch script !

# Settings

Look at create_server_cert.cmd for configuration details.

# Result

As result, the server certificate will be created at "pub" directory:
- server_cert.key - server certificate's key
- server_cert.p12 - pkcs#12 server certificate's container with full root chain (CA, IM CA) included
- server_cert.pem - server certificate in PEM form
- server_cert_full_chain_with_key.pem - server certificate in PEM form with private key and full root chain (CA, IM CA) included
- server_cert_full_chain_without_key.pem - server certificate in PEM form with full root chain (CA, IM CA) included
- server_cert_roots_only.pem - server certificate's full root chain (CA, IM CA) only
