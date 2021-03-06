## /config/app/proxy/forwardProxy/<name>/serviceHttp/keepAliveTimeout

Close the forward proxy TCP connection if there is no HTTP activity in this
amount of time.

Use

If there are no active HTTP transactions (that is, no active requests or
responses) to a server for the specified time (in seconds), the system closes
the TCP connection to the server, reclaiming resources. This can help avoid
problems that some HTTP servers have when connections are kept open
indefinitely.

Setting this to a value of 0 disables the timeout, which directs the system
not to close server TCP connections due to this timeout.

### Parameters

name: Name of forward proxy object

### Data Key

The data key contains the number of seconds (can be fractional).

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

double

#### Default Data Value

0.0

An object uses the default data value when one of the following is true:

  * For objects without bases--When the object's default key is true.
  * For objects with bases--When the object's default key is true, and when the default key is true for all of the object's bases.

### Default Allowed

True

### Request Methods

GET, PUT

### Related

REST API Reference - [/config/app/proxy/forwardProxy](https://docs.lineratesys
tems.com/093Release_2.5/250REST_API_Reference_Guide/config/app/proxy/forwardPr
oxy)

CLI Reference - [Forward Proxy Mode Commands](https://docs.lineratesystems.com
/093Release_2.5/200CLI_Reference_Guide/Configure_Commands/Forward_Proxy_Mode_C
ommands)

### Examples

GET

curl -b cookie.jar -k https://host-117:8443/lrs/api/v1.0/config/app/proxy/forw
ardProxy/fp-01/serviceHttp/keepAliveTimeout

GET Response

    
    {"/config/app/proxy/forwardProxy/fp-01/serviceHttp/keepAliveTimeout": {"default": True,
                                                                            "defaultAllowed": True,
                                                                            "deleteAllowed": False,
                                                                            "numChildren": 0,
                                                                            "type": "double"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/config/app/proxy/forwardProxy/fp-01/serviceHttp/keepAliveTimeout"}
    

PUT

curl -b cookie.jar --data @data.json -k -H "Content-Type: application/json" -X
PUT https://host-117:8443/lrs/api/v1.0/config/app/proxy/forwardProxy/fp-01/ser
viceHttp/keepAliveTimeout

PUT Response

    
    {"httpResponseCode": 200,
      "requestPath": "/config/app/proxy/forwardProxy/fp-01/serviceHttp/keepAliveTimeout",
      "recurse":false}

  1. /config/app/proxy/forwardProxy/<name>/serviceHttp/keepAliveTimeout
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Default Allowed
    4. Request Methods
    5. Related
    6. Examples

