## /status/app/proxy/stats/data/virtualIP/<name>/httpInternalResp403

Use

Use to view the number of HTTP responses with response code 403 sent to the
clients.

### Parameters

name: Name of virtual IP

### Data Key

The data key contains the number of responses.

#### Data Type

uint64

#### Default Data Value

0

### Request Methods

GET

### Related

[CLI Reference - Show Virtual IP Commands](https://docs.lineratesystems.com/09
3Release_2.5/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Virtual_I
P_Commands)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/app/proxy/stat
s/data/virtualIP/vip1/httpInternalResp403

GET Response

    
    {"/status/app/proxy/stats/data/virtualIP/vip1/httpInternalResp403": {"data": 0,
                                                                            "default": False,
                                                                            "defaultAllowed": False,
                                                                            "deleteAllowed": False,
                                                                            "numChildren": 0,
                                                                            "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/virtualIP/vip1/httpInternalResp403"}
    

  1. /status/app/proxy/stats/data/virtualIP/<name>/httpInternalResp403
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

