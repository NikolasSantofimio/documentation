# Servicio AppVersion - Billetera Compensar

El servicio **AppVersion** permite validar si la aplicación móvil de **Billetera Compensar** está actualizada.

## Propósito
Este servicio se utiliza para:
- Verificar la versión instalada de la aplicación.
- Forzar actualizaciones en caso de que se detecte una versión antigua.
- Garantizar compatibilidad con cambios críticos en el backend.

## Flujo básico
1. La app envía la información de su versión actual.
2. El backend compara contra los valores configurados en DynamoDB.
3. Si hay una versión más reciente, responde con la acción requerida (`update_required`, `optional_update`, etc.).

## Componentes relacionados
- **Base de datos**: DynamoDB (`AppVersionTable`).
- **API Gateway**: `walletCommon`.
- **Aplicaciones**: Billetera Compensar.
