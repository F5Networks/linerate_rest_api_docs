## /config/system/interface/<intf_name>/carp/<vhid>/ip

The nodes below this one perform the functions described in this function
overview.

Use

Use to configure the IPv4 or IPv6 address for the CARP group. This is the
address for which this VHID will manage failover.

For IPv6, the physical interface must have an IPv6 address and the CARP IP
address must be within the subnet of the physical interface's IPv6 address.

### Parameters

intf_name: Name of interface

vhid: Virtual Host ID (VHID) used to identify the CARP group

#### Data Type

subtree

### Request Methods

GET

### Related

[REST API Reference - /config/system/interface](https://docs.lineratesystems.c
om/093Release_2.5/250REST_API_Reference_Guide/config/system/interface)

[CLI Reference - Interface Mode Commands](https://docs.lineratesystems.com/093
Release_2.5/200CLI_Reference_Guide/Configure_Commands/Interface_Mode_Commands)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/config/system/interface/em1/carp/1/ip

GET Response

    
    {"/config/system/interface/em1/carp/1/ip": {"data": None,
                                                 "default": False,
                                                 "defaultAllowed": False,
                                                 "deleteAllowed": False,
                                                 "numChildren": 1,
                                                 "type": "subtree"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/config/system/interface/em1/carp/1/ip"}
    

GET (list children)

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/config/system/interfa
ce/em1/carp/1/ip?op=list

GET Response

    
    {"/config/system/interface/em1/carp/1/ip": {"children": {"/config/system/interface/em1/carp/1/ip/addrMask": {"default": False,
                                                                                                                    "defaultAllowed": False,
                                                                                                                    "deleteAllowed": False,
                                                                                                                    "numChildren": 0,
                                                                                                                    "type": "subtree"}},
                                                 "default": False,
                                                 "defaultAllowed": False,
                                                 "deleteAllowed": False,
                                                 "numChildren": 1,
                                                 "type": "subtree"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/config/system/interface/em1/carp/1/ip"}
    

GET (recursively list children)

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/config/system/interfa
ce/em1/carp/1/ip?level=recurse

  1. /config/system/interface/<intf_name>/carp/<vhid>/ip
    1. Parameters
      1. Data Type
    2. Request Methods
    3. Related
    4. Examples

