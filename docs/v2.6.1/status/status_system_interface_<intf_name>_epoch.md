## /status/system/interface/<intf_name>/epoch

Use

Use the view the amount of time elapsed from the system start to the interface
creation, in seconds. This typically shows 0 - 2.

### Parameters

intf_name: Name of interface

### Data Key

The data key contains the number of seconds.

#### Data Type

uint64

### Request Methods

GET

### Related

[REST API Reference - /config/system/interface](https://docs.lineratesystems.c
om/087Release_2.6/250REST_API_Reference_Guide/config/system/interface)

[CLI Reference - Interface Mode Commands](https://docs.lineratesystems.com/087
Release_2.6/200CLI_Reference_Guide/Configure_Commands/Interface_Mode_Commands)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/status/system/interface/em1/epoch

GET Response

    
    {"/status/system/interface/em1/epoch": {"data": 1,
                                             "default": False,
                                             "defaultAllowed": False,
                                             "deleteAllowed": False,
                                             "numChildren": 0,
                                             "type": "uint64"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/system/interface/em1/epoch"}
    

  1. /status/system/interface/<intf_name>/epoch
    1. Parameters
    2. Data Key
      1. Data Type
    3. Request Methods
    4. Related
    5. Examples

