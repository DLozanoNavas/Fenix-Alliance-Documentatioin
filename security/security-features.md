# Security Features

### Encryption at rest <a id="encryption-at-rest"></a>

All files sended to our applications are automatically encrypted with a 256-bit Advanced Encryption Standard \(AES\) cipher. SSE automatically encrypts data when writing it to Storage. When you read your files, our storage decrypts the data before returning it. This process incurs no additional charges and doesn't degrade performance. This feature can't be disabled.

### Encryption in transit <a id="encryption-in-transit"></a>

We keep your data secure by enabling _transport-level security_ between our applications and the client. We ALWAYS use _HTTPS_ to secure communication over the public internet. When you call the REST APIs to access objects in storage accounts or our databases, we enforce the use of HTTPS by requiring secure transfer and connections that use HTTP will be refused and redirected.

