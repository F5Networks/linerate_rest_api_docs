## /status/app/proxy/stats/data/virtualServer/<name>/sslSessionIdPersistenceEv
ictedPerSec5MinAvg

Use

Use to view the 5-minute average of the number of SSL Session ID persistence
cache entries evicted due to cache being full.

### Parameters

name: Name of virtual server object

### Data Key

The data key contains the number of cache entries evicted.

#### Data Type

uint64

#### Default Data Value

0

### Request Methods

GET

### Related

CLI Reference - [Show Virtual Server Commands](https://docs.lineratesystems.co
m/093Release_2.5/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Virtu
al_Server_Commands)

### Examples

GET

curl -b cookie.jar -k https://host-51:8443/lrs/api/v1.0/status/app/proxy/stats
/data/virtualServer/vs-01/sslSessionIdPersistenceEvictedPerSec5MinAvg

GET Response

    
    {"/status/app/proxy/stats/data/virtualServer/vs-01/sslSessionIdPersistenceEvictedPerSec5MinAvg": {"data": 0,
                                                                                                       "default": False,
                                                                                                       "defaultAllowed": False,
                                                                                                       "deleteAllowed": False,
                                                                                                       "numChildren": 0,
                                                                                                       "redacted": False,
                                                                                                       "sensitive": False,
                                                                                                       "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/virtualServer/vs-01/sslSessionIdPersistenceEvictedPerSec5MinAvg"}
    

  1. /status/app/proxy/stats/data/virtualServer/<name>/sslSessionIdPersistenceEvictedPerSec5MinAvg
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

