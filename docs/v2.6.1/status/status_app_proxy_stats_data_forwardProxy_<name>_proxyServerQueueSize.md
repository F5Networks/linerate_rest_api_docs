## /status/app/proxy/stats/data/forwardProxy/<name>/proxyServerQueueSize

Use

Use to view the number of HTTP client requests in the HTTP load balancer mode
and the number of client connections in the L4 load balancer mode that are in
the queue at the real server. This is the number of HTTP requests for which an
entire response has not yet been received from the server and the number of
client connections pending to be connected to an origin server.

These numbers are highly variable and change in very small time frames.
Because these values are not averages, but are instantaneous measurements,
they are subject to sampling error. For a more meaningful view, use the the
proxyServerQueueSize1MinAvg or proxyServerQueueSize5MinAvg statistics.

### Parameters

name: Name of forward proxy object

### Data Key

The data key contains the number of requests.

#### Data Type

int32

#### Default Data Value

0

### Request Methods

GET

### Related

CLI Reference - [Show Forward Proxy Commands](https://docs.lineratesystems.com
/087Release_2.6/200CLI_Reference_Guide/Exec_Commands/Show_Commands/Show_Forwar
d_Proxy_Commands)

### Examples

GET

curl -b cookie.jar -k https://host-70:8443/lrs/api/v1.0/status/app/proxy/stats
/data/forwardProxy/fp-01/proxyServerQueueSize

GET Response

    
    
    {"/status/app/proxy/stats/data/forwardProxy/fp-01/proxyServerQueueSize": {"data": 0,
                                                                               "default": False,
                                                                               "defaultAllowed": False,
                                                                               "deleteAllowed": False,
                                                                               "numChildren": 0,
                                                                               "type": "int32"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/status/app/proxy/stats/data/forwardProxy/fp-01/proxyServerQueueSize"}
    

  1. /status/app/proxy/stats/data/forwardProxy/<name>/proxyServerQueueSize
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

