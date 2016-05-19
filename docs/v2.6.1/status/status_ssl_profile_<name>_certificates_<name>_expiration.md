## /status/ssl/profile/<name>/certificates/<name>/expiration

Use

Use to view the certificate's expiration date.

### Parameters

name: Name of SSL profile

name: Name of certificates object

### Data Key

The data key contains the expiration date.

#### Data Type

string

#### Default Data Value

""

### Request Methods

GET

### Related

REST API Reference - [/status/ssl](https://docs.lineratesystems.com/087Release
_2.6/250REST_API_Reference_Guide/status/ssl)

[CLI Reference - Show SSL Commands](/087Release_2.6/200CLI_Reference_Guide/Exe
c_Commands/Show_Commands/Show_SSL_Commands)

### Examples

GET

curl -b cookie.jar -k https://host-128:8443/lrs/api/v1.0/status/ssl/profile/sp
-01/certificates/name/expiration

  1. /status/ssl/profile/<name>/certificates/<name>/expiration
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples
