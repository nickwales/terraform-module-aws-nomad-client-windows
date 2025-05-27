## Windows Nomad Client AWS

This module will create a Windows Nomad client on AWS 


### Debugging

The user data script is somewhere in a directory on this path:

`C:\Windows\System32\config\systemprofile\AppData\Local\Temp\EC2Launch*`

### Issues making the certificate in the userdata script.

## Create the certificate variable with

```
$cert = @{
>> -----BEGIN CERTIFICATE-----
>> ...
>> -----END CERTIFICATE-----
>> }

$cert | Out-File -FilePath C:\consul\certs\consul-agent-ca.pem -Encoding Ascii
```


### Basic Windows Commands

Because I forget

`Start-Service -name consul`

`Get-Service -name consul`