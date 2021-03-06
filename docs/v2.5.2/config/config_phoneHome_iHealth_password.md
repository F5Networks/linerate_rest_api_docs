## /config/phoneHome/iHealth/password

Use

Use to configure the F5 password, which you created when you downloaded the
installation file, for the Starter Edition license and to send phone home
data. You must configure the username node first.

Normally, you should use the clear form of the password, and the system
encrypts the password. You can see the encrypted password the following ways:

  * CLI command--show run
  * REST API--/config/phonehome/ihealth/password

Use the encrypted form of the password only when you need to use an existing
password on another system. You can copy the encrypted password from the show
run output or from the /status/config/running node, then paste it into the
encrypted form of the command on another system.

### Data Key

The data key contains the password.

Note: When the default key is set to true, it means the object is set to its
default. In this case, the system works as follows:

  * On a PUT operation, the system ignores the data key. (Applicable only to /config nodes.)
  * On a GET operation, the response only contains "default": True and does not contain the data key.
  * If the object has a base, it inherits its setting from its base.

See [Setting Objects to Their Default](https://docs.lineratesystems.com/093Rel
ease_2.5/250REST_API_Reference_Guide/000Getting_Started_with_the_REST_API/300U
nderstanding_the_REST_Hierarchy#Setting_Objects_to_Their_Default_(Default_Key)
).

#### Data Type

string

#### Default Data Value

""

An object uses the default data value when one of the following is true:

  * For objects without bases--When the object's default key is true.
  * For objects with bases--When the object's default key is true, and when the default key is true for all of the object's bases.

### Default Allowed

True

### Request Methods

GET, PUT

### Related

REST API Reference - [/config/phoneHome](https://docs.lineratesystems.com/093R
elease_2.5/250REST_API_Reference_Guide/config/phoneHome)

REST API Reference - [/status/app/phoneHome](https://docs.lineratesystems.com/
093Release_2.5/250REST_API_Reference_Guide/status/app/phoneHome)

CLI Reference - [Phone Home Mode Commands](https://docs.lineratesystems.com/09
3Release_2.5/200CLI_Reference_Guide/Configure_Commands/Phone_Home_Mode_Command
s)

### Examples

GET

curl -b cookie.jar -k
https://10.1.2.3:8443/lrs/api/v1.0/config/phoneHome/iHealth/password

GET Response

    
    
    {"/config/phoneHome/iHealth/password": {"default": True,
                                             "defaultAllowed": True,
                                             "deleteAllowed": False,
                                             "numChildren": 0,
                                             "type": "string"},
     "httpResponseCode": 200,
     "recurse": False,
     "requestPath": "/config/phoneHome/iHealth/password"}
    

PUT

curl -b cookie.jar --data @data.json -k -H "Content-Type: application/json" -X
PUT https://10.1.2.3:8443/lrs/api/v1.0/config/phoneHome/iHealth/password

PUT Response

    
    
    {"httpResponseCode": 200,
      "requestPath": "/config/phoneHome/iHealth/password",
      "recurse":false}

  1. /config/phoneHome/iHealth/password
    1. Data Key
      1. Data Type
      2. Default Data Value
    2. Default Allowed
    3. Request Methods
    4. Related
    5. Examples

