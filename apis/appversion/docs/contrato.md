# Contrato del API AppVersion

## Método y URL
- **Método**: `POST`
- **Recurso**: `/appversion`
- **Content-Type**: `application/json`

## Request
```json
{
  "majorVersion": 2,
  "minorVersion": 5,
  "release": 12,
  "client": "compensar",
  "store": "playstore"
}
