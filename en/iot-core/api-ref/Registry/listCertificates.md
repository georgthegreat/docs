---
editable: false
sourcePath: en/_api-ref/iot/devices/api-ref/Registry/listCertificates.md
---

# IoT Core Service, REST: Registry.listCertificates
Retrieves the list of registry certificates for the specified registry.
 

 
## HTTP request {#https-request}
```
GET https://iot-devices.{{ api-host }}/iot-devices/v1/registries/{registryId}/certificates
```
 
## Path parameters {#path_params}
 
Parameter | Description
--- | ---
registryId | <p>Required. ID of the registry to list certificates for.</p> <p>The maximum string length in characters is 50.</p> 
 
## Response {#responses}
**HTTP Code: 200 - OK**

```json 
{
  "certificates": [
    {
      "registryId": "string",
      "fingerprint": "string",
      "certificateData": "string",
      "createdAt": "string"
    }
  ]
}
```

 
Field | Description
--- | ---
certificates[] | **object**<br><p>List of certificates for the specified registry.</p> 
certificates[].<br>registryId | **string**<br><p>ID of the registry that the certificate belongs to.</p> 
certificates[].<br>fingerprint | **string**<br><p>SHA256 hash of the certificates.</p> 
certificates[].<br>certificateData | **string**<br><p>Public part of the certificate.</p> 
certificates[].<br>createdAt | **string** (date-time)<br><p>Creation timestamp.</p> <p>String in <a href="https://www.ietf.org/rfc/rfc3339.txt">RFC3339</a> text format. The range of possible values is from ``0001-01-01T00:00:00Z`` to ``9999-12-31T23:59:59.999999999Z``, i.e. from 0 to 9 digits for fractions of a second.</p> <p>To work with values in this field, use the APIs described in the <a href="https://developers.google.com/protocol-buffers/docs/reference/overview">Protocol Buffers reference</a>. In some languages, built-in datetime utilities do not support nanosecond precision (9 digits).</p> 