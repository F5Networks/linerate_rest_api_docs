##
/status/app/proxy/stats/data/forwardProxy/<name>/httpProxyServerRespAbandoned

Use

Use to view the number of HTTP responses from the server that were discarded
without sending to the clients.

### Parameters

name: Name of forward proxy object

### Data Key

The data key contains the number of responses.

#### Data Type

uint64

#### Default Data Value

0

### Request Methods

GET

### Related

CLI Reference - [Show Forward Proxy Commands](https://docs.lineratesystems.com
/087Release_2.6/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Forwar
d_Proxy_Commands)

### Examples

GET

curl -b cookie.jar -k https://host-70:8443/lrs/api/v1.0/status/app/proxy/stats
/data/forwardProxy/fp-01/httpProxyServerRespAbandoned

GET Response

    
    {"/status/app/proxy/stats/data/forwardProxy/fp-01/httpProxyServerRespAbandoned": {"data": 0,
                                                                                       "default": False,
                                                                                       "defaultAllowed": False,
                                                                                       "deleteAllowed": False,
                                                                                       "numChildren": 0,
                                                                                       "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/forwardProxy/fp-01/httpProxyServerRespAbandoned"}
    

  1. /status/app/proxy/stats/data/forwardProxy/<name>/httpProxyServerRespAbandoned
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples
