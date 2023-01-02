[Home](../README.md)

# Class 17

## AWS Cont'd

### AWS S3

- AWS S3 is AWS Simple Storage Service. It has many use cases, including remote file storage with availability needs ranging from immediate to maybe once or twice a year. It offers incredible durability assurance and guarantees high availability for it's services that require it.

### Lambda

- AWS Lambda is AWS's serverless function provider. This means that the code is run directly, without being hosted on a dedicated server. It is extremely cheap for most use cases and is very useful for things like real-time file-processing, where an action such as a file upload should trigger something to happen to that file, and then possibly output something to a destination, such as sending a notification email.

### CDN

- A CDN is a content delivery network and uses cacheing to maintain quick access to data.  
- When a visitor requests some resource, the CDN checks if that resource is already cached. If so, it serves the resource, and if not, it requests it from the original source, caches it, and then serves it to the visitor.
- This is very useful for serving commonly accessed data.
- It can also prevent certain types of malicious behavior, such as a DDoS, or distributed denial of service attack, where your site is flooded  with so much traffic that the server crashes. The CDN is able to serve it resources extremely quickly, and it does not access the resource origin if the resource is already cached, which both work together to mean that a DDoS attack never impacts the origin (your site).
