## /config/ssl/profile/<name>/sessCacheMode

Set session cache memory size.

Use

Use to improve performance for SSL connections by storing session keys. The
system saves and can reuse an SSL session key for client connections. The
cached session key lets the system establish the SSL connection to the same
client, bypassing the normal SSL handshake process.

This applies to SSL termination only. You set the amount of system RAM you
want to use to store session keys. To determine the space needed to use
session keys effectively, consider the following:

  * The more active clients you have, the more space you need for the keys, which are generally about 2 KiB.

  * To be beneficial, the cache must be large enough to store session keys between connections from the same client.

  * Consider how many connections per second you expect and how much time you expect between the same client connecting multiple times.

In a failover situation, where the primary system fails over to a secondary
system, the session cache is not copied to the secondary system.

You can use both session cache and session tickets at the same time. If the
client supports session tickets, the system uses the session ticket. If the
client does not support session tickets, the system uses session cache.

### Parameters

name: Name of SSL profile

### Data Key

The data key contains one of the values defined in Data Values below.

Note: When the default key is set to true, it means the object is set to its
default. In this case, the system works as follows:

  * On a PUT operation, the system ignores the data key. (Applicable only to /config nodes.)
  * On a GET operation, the response only contains "default": True and does not contain the data key.
  * If the object has a base, it inherits its setting from its base.

See [Setting Objects to Their Default](https://docs.lineratesystems.com/093Rel
ease_2.5/250REST_API_Reference_Guide/000Getting_Started_with_the_REST_API/300U
nderstanding_the_REST_Hierarchy#Setting_Objects_to_Their_Default_(Default_Key)
).

#### Data Type

uint32

#### Data Values

0 (No cache; cache disabled, sessCacheSize node ignored)

1 (Auto size and currently is set to 10 MB [10485760 bytes]; sessCacheSize
node ignored)

2 (Explicit size; uses the size from the sessCacheSize node)

#### Default Data Value

0

An object uses the default data value when one of the following is true:

  * For objects without bases--When the object's default key is true.
  * For objects with bases--When the object's default key is true, and when the default key is true for all of the object's bases.

### Default Allowed

True

### Request Methods

GET, PUT

### Related

[REST API Reference - /config/ssl](https://docs.lineratesystems.com/093Release
_2.5/250REST_API_Reference_Guide/config/ssl)

[CLI Reference - SSL Mode Commands](https://docs.lineratesystems.com/093Releas
e_2.5/200CLI_Reference_Guide/Configure_Commands/SSL_Mode_Commands)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/config/ssl/profile/sp-01/sessCacheMode

GET Response

    
    {"/config/ssl/profile/sp-01/sessCacheMode": {"data": 1,
                                                  "default": False,
                                                  "defaultAllowed": True,
                                                  "deleteAllowed": False,
                                                  "numChildren": 0,
                                                  "type": "uint32"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/config/ssl/profile/sp-01/sessCacheMode"}
    

PUT

curl -b cookie.jar --data @data.json -k -H "Content-Type: application/json" -X
PUT https://10.1.2.3:8443/lrs/api/v1.0/config/ssl/profile/sp-01/sessCacheMode

PUT Response

    
    {"httpResponseCode": 200,
      "requestPath": "/config/ssl/profile/sp-01/sessCacheMode",
      "recurse":false}

  1. /config/ssl/profile/<name>/sessCacheMode
    1. Parameters
    2. Data Key
      1. Data Type
      2. Data Values
      3. Default Data Value
    3. Default Allowed
    4. Request Methods
    5. Related
    6. Examples

