## /status/app/proxy/stats/data/global/virtualServer/proxyServerL4ConnSuccessf
ulPerSec1MinAvg

Use

Use to view the 1-minute average of the number of L4 connection requests per
second made to the servers due to L4 client connection requests that were
successful.

### Data Key

The data key contains the 1-minute average.

#### Data Type

uint64

#### Default Data Value

0

### Request Methods

GET

### Related

CLI Reference - [Show Proxy Commands](/087Release_2.6/200CLI_Reference_Guide/E
xec_Commands/Show_Commands/Show_Proxy_Commands)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/app/proxy/stat
s/data/global/virtualServer/proxyServerL4ConnSuccessfulPerSec1MinAvg

GET Response

    
    
    {"/status/app/proxy/stats/data/global/virtualServer/proxyServerL4ConnSuccessfulPerSec1MinAvg": {"data": 0,
                                                                                                     "default": False,
                                                                                                     "defaultAllowed": False,
                                                                                                     "deleteAllowed": False,
                                                                                                     "numChildren": 0,
                                                                                                     "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/global/virtualServer/proxyServerL4ConnSuccessfulPerSec1MinAvg"}
    

  1. /status/app/proxy/stats/data/global/virtualServer/proxyServerL4ConnSuccessfulPerSec1MinAvg
    1. Data Key
      1. Data Type
      2. Default Data Value
    2. Request Methods
    3. Related
    4. Examples

