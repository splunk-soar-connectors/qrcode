[comment]: # "Auto-generated SOAR connector documentation"
# QR Code

Publisher: Splunk Community  
Connector Version: 1.0.1  
Product Vendor: OpenCV  
Product Name: OpenCV  
Product Version Supported (regex): ".\*"  
Minimum Product Version: 5.3.2.88192  

Extract Data from QR Codes

# Splunk> Phantom

Welcome to the open-source repository for Splunk> Phantom's qrcode App.

Please have a look at our [Contributing Guide](https://github.com/Splunk-SOAR-Apps/.github/blob/main/.github/CONTRIBUTING.md) if you are interested in contributing, raising issues, or learning more about open-source Phantom apps.

## Legal and License

This Phantom App is licensed under the Apache 2.0 license. Please see our [Contributing Guide](https://github.com/Splunk-SOAR-Apps/.github/blob/main/.github/CONTRIBUTING.md#legal-notice) for further details.


### Supported Actions  
[test connectivity](#action-test-connectivity) - Validate the asset configuration for connectivity using supplied configuration  
[decode qr code](#action-decode-qr-code) - Decodes a PNG containing a QR code  

## action: 'test connectivity'
Validate the asset configuration for connectivity using supplied configuration

Type: **test**  
Read only: **True**

#### Action Parameters
No parameters are required for this action

#### Action Output
No Output  

## action: 'decode qr code'
Decodes a PNG containing a QR code

Type: **generic**  
Read only: **False**

#### Action Parameters
PARAMETER | REQUIRED | DESCRIPTION | TYPE | CONTAINS
--------- | -------- | ----------- | ---- | --------
**vault_id** |  required  | Vault ID of the PNG file | string |  `vault id` 

#### Action Output
DATA PATH | TYPE | CONTAINS | EXAMPLE VALUES
--------- | ---- | -------- | --------------
action_result.parameter.vault_id | string |  `vault id`  |  
action_result.status | string |  |   success  failed 
action_result.data.\*.output | string |  |  
action_result.message | string |  |  
summary.total_objects | numeric |  |  
summary.total_objects_successful | numeric |  |  