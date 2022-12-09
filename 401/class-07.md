[Home](../README.md)

# Class 7

## Bearer Authorization

### Intro to JWT

- JSON Web Token is an open standard that defines a lightweight way to securely transmit information between two parties
- JWTs are used for authorization to access protected routes once and entity has been authenticated
- Claims are expected in the middle part of a JWT. The first part is the encoded header and the final part is the signature.

### Are JWTs Secure?

- Although anyone can decode the payload, they cannot change it without invalidating the signature, which takes into account the header and payload. If the header, payload, and secret do not hash to create the same signature presented, then the JWT is invalid
- In order for this to work, both sender and receiver must know the secret used to create the signature.
- Because teh concatenated content and secret are hashed, we cannot decipher what they were from the signature alone. The way we verify validity is to recreate the hash with the same concatenated content and secret and check to see that it produces the same result as the signature presented.
- Alice and Bob both know secret S, but Charlie doesn't. Alice can send Bob a JWT consisting of some content, A, and a signaure, sA, produced by Hash(A + S). Bob recieves and can verify that it is from Alice by also doing Hash(A + S). Since that matches sA, he knows that content A is valid. Charlie tries to impersonate Alice, but since he doesn't know the secret, the best he can do is just hash the content, or guess the secret. So he sends content C, along with signature sC creaed by Hash(C + badSecret). Bob receives it and checks the token by doing Hash(C + S), and finds it produces something different from sC. He knows now that the token is invalid.

### JWTs Described

- JWTs are used because they can securely transmit information in a manner that ensures to the receiver the validity of the sender.
- since JWTs are compact and self-contained, they rely on little other information besides the secret used to validate, and they also create very little overhead to the requests sent.
- The three components are the base64 encoded header, base64 encoded payload, and the hashed signature.
