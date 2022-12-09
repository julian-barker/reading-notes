[Home](../README.md)

# Class 6

## Securing Passwords

- We can safely hash and store a password by hashing with a strong algorithm to create a fixed-length representation of the password that cannot be reversed to reveal the original password. From there, we store the hashed value and recalculate it every time we are presented with a password to check it against the stored hash.
  - A always gets hashed to B, but B cannot be used to get back to A. We store B and then compare it with the hash of a given password. If the hash matches B, then the password provided *must (barring hash collisions) be equal to A

- Bcrypt is a hashing algorithm that was created to safeguard against the weaknesses of some other alogrithms.
- A good reason to use it is that is has a built in  work factor that determines how difficult / slow it is to perform the hash algorithm, thus making it relatively future-proof.

## Basic Auth

- HTTP Basic Authentication is the simplest way of enforcing access control and involves simply sending a username and password in the Authorization header of an http request.
- It provides no confidentiality with respect to the credentials sent over the request, and is thus not secure. For this reason, it is used with HTTPS.
- The authorization header is sent in the form `basic <username>:<password>` and is base64 encoded.

## OWASP Cheatsheet

- Authentication is the process by which a system verifies the identity of the entity interacting with it. This frequently happens through username and password. Authentication subsequently leads to authorization, which determines which resources that verified entity may access.
- Error message responses should remain generic so as to not provide any information to a malicious actor that could hint at specifics of the system internals and how to bypass them.
