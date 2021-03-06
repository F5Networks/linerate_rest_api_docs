## /status/app/proxy/stats/data/global/virtualServer/sslSessionIdPersistenceCa
cheMissesPerSec

Use

Use to view the number of misses in SSL Session ID persistence cache.

### Data Key

The data key contains the number of misses.

#### Data Type

uint64

#### Default Data Value

0

### Request Methods

GET

### Related

CLI Reference - [Show Virtual Server Commands](https://docs.lineratesystems.co
m/087Release_2.6/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Virtu
al_Server_Commands)

### Examples

GET

curl -b cookie.jar -k https://host-51:8443/lrs/api/v1.0/status/app/proxy/stats
/data/global/virtualServer/sslSessionIdPersistenceCacheMissesPerSec

GET Response

    
    {"/status/app/proxy/stats/data/global/virtualServer/sslSessionIdPersistenceCacheMissesPerSec": {"data": 0,
                                                                                                     "default": False,
                                                                                                     "defaultAllowed": False,
                                                                                                     "deleteAllowed": False,
                                                                                                     "numChildren": 0,
                                                                                                     "redacted": False,
                                                                                                     "sensitive": False,
                                                                                                     "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/global/virtualServer/sslSessionIdPersistenceCacheMissesPerSec"}
    

  1. /status/app/proxy/stats/data/global/virtualServer/sslSessionIdPersistenceCacheMissesPerSec
    1. Data Key
      1. Data Type
      2. Default Data Value
    2. Request Methods
    3. Related
    4. Examples

