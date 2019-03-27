# webauthn-sw-example

This is a simple example showing how the [webauth-service-worker](https://github.com/joaosantos15/webauthn-sw) and [webauth-service-worker-client](https://github.com/joaosantos15/webauthn-ws-client) modules can be used. 

These modules leverage some of the features of the browser WebAuthn API to store a secret on the client side hardware, in the `userHandle` field. Apps can then use that secret as a login secret.

⚠️ Note that **this is not** the way WebAuthn was designed to be used, and using the `userHandle` field to store a secret is not recomended by the specification -- it's just a fun little hack we put together.

## Setup

```sh
> npm install
> npm run start # this build and starts a web server on port 8080
```

## Trying it out

Go to [`http://localhost:8080`](http://localhost:8080), register and login.
