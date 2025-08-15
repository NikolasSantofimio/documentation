# Ambientes del servicio AppVersion

## Desarrollo
- **URL**: `https://dev-api.example.com/appversion`
- **API Key**: `AWS_SSM_PARAM:/wallet/api/dev/appversion/key`

## QA
- **URL**: `https://qa-api.example.com/appversion`
- **API Key**: `AWS_SSM_PARAM:/wallet/api/qa/appversion/key`

## Producción
- **URL**: `https://api.example.com/appversion`
- **API Key**: `AWS_SSM_PARAM:/wallet/api/prod/appversion/key`

> 🔒 Las API Keys se almacenan en AWS SSM Parameter Store y no se exponen en este documento.
