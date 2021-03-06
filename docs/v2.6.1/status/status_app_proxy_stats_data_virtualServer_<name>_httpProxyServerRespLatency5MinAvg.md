## /status/app/proxy/stats/data/virtualServer/<name>/httpProxyServerRespLatenc
y5MinAvg

Use

Use to view the 5-minute average of the average time between receiving the
first and last bytes of the response.

### Parameters

name: Name of virtual server object

### Data Key

The data key contains the 5-minute average.

#### Data Type

double

### Request Methods

GET

### Related

CLI Reference - [Show Virtual Server Commands](https://docs.lineratesystems.co
m/087Release_2.6/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Virtu
al_Server_Commands)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/app/proxy/stat
s/data/virtualServer/vs-01/httpProxyServerRespLatency5MinAvg

GET Response

    
    
    {"/status/app/proxy/stats/data/virtualServer/vs-01/httpProxyServerRespLatency5MinAvg": {"data": 0.0,
                                                                                          "default": False,
                                                                                          "defaultAllowed": False,
                                                                                          "deleteAllowed": False,
                                                                                          "numChildren": 0,
                                                                                          "type": "double"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/virtualServer/vs-01/httpProxyServerRespLatency5MinAvg"}
    

  1. /status/app/proxy/stats/data/virtualServer/<name>/httpProxyServerRespLatency5MinAvg
    1. Parameters
    2. Data Key
      1. Data Type
    3. Request Methods
    4. Related
    5. Examples

