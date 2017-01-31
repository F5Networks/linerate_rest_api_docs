## /status/system/interface/<intf_name>/ip/v6LinkLocal

Use

Use to view whether the IPv6 address is link-local.

### Parameters

intf_name: Name of interface

### Data Key

The data key contains the link-local IPv6 address.

#### Data Type

ip-addr-with-mask

### Default Allowed

False

### Request Methods

GET

### Related

REST API Reference - [/config/system/interface](/087Release_2.6/250REST_API_Re
ference_Guide/config/system/interface)

CLI Reference - [Show Interfaces Commands](/087Release_2.6/200CLI_Reference_Gu
ide/Exec_Commands/Show_Commands/Show_Interfaces_Commands)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/status/system/interface/em1/ip/v6LinkLocal

GET Response

    
    
    {"/status/system/interface/em1/ip/v6LinkLocal": {"data": None,
                                                      "default": False,
                                                      "defaultAllowed": False,
                                                      "deleteAllowed": False,
                                                      "numChildren": 1,
                                                      "type": "ip-addr-with-mask"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/system/interface/em1/ip/v6LinkLocal"}
    

  1. /status/system/interface/<intf_name>/ip/v6LinkLocal
    1. Parameters
    2. Data Key
      1. Data Type
    3. Default Allowed
    4. Request Methods
    5. Related
    6. Examples
