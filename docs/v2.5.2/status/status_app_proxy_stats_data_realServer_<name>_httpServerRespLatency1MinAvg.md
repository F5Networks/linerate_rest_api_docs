## /status/app/proxy/stats/data/realServer/<name>/httpServerRespLatency1MinAvg

Use

Use to view the 1-minute average of the average time between receiving the
first and last bytes of the response.

### Parameters

name: Name of real server

### Data Key

The data key contains the time in seconds.

#### Data Type

double

#### Default Data Value

0

### Request Methods

GET

### Related

[CLI Reference - Show Real Server Commands](https://docs.lineratesystems.com/0
93Release_2.5/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Real_Ser
ver_Commands)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/app/proxy/stat
s/data/realServer/rs1/httpServerRespLatency1MinAvg

GET Response

    
    
    {"/status/app/proxy/stats/data/realServer/rs1/httpServerRespLatency1MinAvg": {"data": 0.0,
                                                                                        "default": False,
                                                                                        "defaultAllowed": False,
                                                                                        "deleteAllowed": False,
                                                                                        "numChildren": 0,
                                                                                        "type": "double"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/realServer/rs1/httpServerRespLatency1MinAvg"}
    

  1. /status/app/proxy/stats/data/realServer/<name>/httpServerRespLatency1MinAvg
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

