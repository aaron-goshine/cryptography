### cryptography

Encryption secures messages so that they can be verified as accurate and protected from interception.
Python's cryptography support includes `hashlib` for generating signatures of message content using standard algorithms, such as MD5 and SHA, and `humc` for verifying that a message has not been alerted in transmission.

The `hashlib` module deprecates the separate `md5` and `sha` module and makes their API consistent. To work with a specific hash algorithm, use the appropriate constructor function to create a hash object. From there, the objects use the same API, no matter what algorithm is being used.

Since `hashlib` is "backed" by OpenSSL, all algorithms provided by that library are available, including

- md5
- sha1
- sha224
- sha256
- sha384
- sha512

### Reference materials

##### Hmac
[hmac doc](http://docs.python.org/library/hamac.html)
The standard library documentation for this module.

##### RFC 2104
[rfc2104](http://tools.ietf.org/html/rfc2104.html)
HMAC: keyed-Hashing for Message Authentication.

#### hashlib
The hashlib module provides the hash generators listed above.

#### pickle
Serialization library.

[Authenticating to Amazon S3 Web Service]
(http://docs.amazonwebservices.com/AmazonS3/2006-03-01/index.html?S3_Authentication.html)
Instructions for authenticating to S3 using HMAC-SHA1 singed credentials.

