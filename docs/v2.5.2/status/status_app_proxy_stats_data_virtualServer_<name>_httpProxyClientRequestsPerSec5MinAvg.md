## /status/app/proxy/stats/data/virtualServer/<name>/httpProxyClientRequestsPe
rSec5MinAvg

Use

Use to view the 5 minute average of the number of client HTTP requests per
second received.

### Parameters

name: Name of object

### Data Key

#### Data Type

uint64

### Request Methods

GET

### Related

[REST API Reference - /status/app/proxy/stats](https://docs.lineratesystems.co
m/093Release_2.5/250REST_API_Reference_Guide/status/app/proxy/stats)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/app/proxy/stat
s/data/virtualServer/vs-01/httpProxyClientRequestsPerSec5MinAvg

GET Response

    
    {"/status/app/proxy/stats/data/virtualServer/vs-01/httpProxyClientRequestsPerSec5MinAvg": {"data": 0,
                                                                                             "default": False,
                                                                                             "defaultAllowed": False,
                                                                                             "deleteAllowed": False,
                                                                                             "numChildren": 0,
                                                                                             "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/virtualServer/vs-01/httpProxyClientRequestsPerSec5MinAvg"}
    

  1. /status/app/proxy/stats/data/virtualServer/<name>/httpProxyClientRequestsPerSec5MinAvg
    1. Parameters
    2. Data Key
      1. Data Type
    3. Request Methods
    4. Related
    5. Examples
