## /status/scripting/packages/bundled/<name>/version

Use

Use to view the version of the specified Node Packaged Module that comes
bundled with the scripting tool.

### Parameters

name: Name of bundled object

### Data Key

The data key contains the version.

#### Data Type

string

#### Default Data Value

""

### Request Methods

GET

### Related

REST API Reference - [scripting](https://docs.lineratesystems.com/087Release_2
.6/250REST_API_Reference_Guide/exec/scripting)

CLI Reference - [Scripting Mode Commands](https://docs.lineratesystems.com/087
Release_2.6/200CLI_Reference_Guide/Exec_Commands/Scripting_Mode_Commands)

### Examples

GET

curl -b cookie.jar -k https://10.1.2.3:8443/lrs/api/v1.0/status/scripting/pack
ages/bundled/name/version

GET Response

    
    {"httpResponseCode": 404,
     "internalResponseCode": 101,
     "message": "Request failed: Unable to retrieve data from controller\n  Path: /scripting/packages/bundled/name/version\n  ResponseCode: 101 (Path not found)\n",
     "recurse": False,
     "requestPath": "/status/scripting/packages/bundled/name/version"}
    

  1. /status/scripting/packages/bundled/<name>/version
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

