## /status/scripting/packages/user/<name>/description

Use

Use to view the description of the specified Node Packaged Module that is user
installed.

### Parameters

name: Name of the user-installed Node Packaged Module

### Data Key

The data key contains the description.

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
ages/user/name/description

GET Response

    
    {"httpResponseCode": 404,
     "internalResponseCode": 101,
     "message": "Request failed: Unable to retrieve data from controller\n  Path: /scripting/packages/user/name/description\n  ResponseCode: 101 (Path not found)\n",
     "recurse": False,
     "requestPath": "/status/scripting/packages/user/name/description"}
    

  1. /status/scripting/packages/user/<name>/description
    1. Parameters
    2. Data Key
      1. Data Type
      2. Default Data Value
    3. Request Methods
    4. Related
    5. Examples

