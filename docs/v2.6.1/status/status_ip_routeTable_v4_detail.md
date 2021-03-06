## /status/ip/routeTable/v4/detail

View configured IP4 routes, including kernel routes.

Use

To see IP routes.

  * A connected route (C) is one the system automatically adds based on the interface IP address.
  * A static route (S) is one you created using the ip route command.
  * The detail form of IP routes includes additional internal details about the routing table that you can use for troubleshooting. For example, the detail includes ARP entries.

### Data Key

The data key contains the route summary information, including kernel routes.

#### Data Type

string

#### Default Data Value

""

### Request Methods

GET

### Related

REST API Reference - /config/[ip](https://docs.lineratesystems.com/087Release_
2.6/250REST_API_Reference_Guide/config/ip)

CLI Reference - [Show IP Commands](https://docs.lineratesystems.com/087Release
_2.6/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_IP_Commands)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/status/ip/routeTable/v4/detail

GET Response

    
    {"/status/ip/routeTable/v4/detail": {"data": "\nCodes: C - connected, S - static, K - kernel, M - multicast\n\nGateway of last resort is not set\n\nC    10.126.0.0/16 is directly connected, em0, MTU 1500\nC    10.126.0.1/32 is directly connected, em0, MTU 1500\nC    10.126.1.185/32 is directly connected, em0, MTU 1500\nC    10.126.64.38/32 is directly connected, em0, MTU 1500\nC    10.126.128.20/32 is directly connected, em0, MTU 1500\nS    10.127.0.0/16 via 10.126.0.1, em0, MTU 1500\nKC   127.0.0.1/32 is directly connected, lo0, MTU 16384\nC    201.0.0.0/8 is directly connected, em1, MTU 9000\n",
                                          "default": False,
                                          "defaultAllowed": False,
                                          "deleteAllowed": False,
                                          "numChildren": 0,
                                          "type": "string"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/ip/routeTable/v4/detail"}
    

  1. /status/ip/routeTable/v4/detail
    1. Data Key
      1. Data Type
      2. Default Data Value
    2. Request Methods
    3. Related
    4. Examples

