#  Bearer Authorization
are encoded JSON objects that “bear” or “contain” enough information for the server to assert that any client request that presents a valid token must have originated from a client that has previously authenticated themselves using either Basic or OAuth

1. Bearer Tokens are sent to the user/client after the initial signin process has completed.
2. Clients must make every subsequent request to the server with that token, in the header
3. Authorization: Bearer encoded.jsonwebtoken.here

4. The server opens the token, does the re-authentication, and then grants or denies access
5. In express servers, this can be done in middleware, in conjunction with a user model

# When should you use JSON Web Tokens?

* *Authorization*: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

* *Information Exchange*: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content.
