# Mapeo de campos entre App móvil, Backend AWS y Postilion

Este documento describe cómo se mueven y transforman los datos entre los diferentes sistemas.

---

## Flujo general

1. El **App móvil** envía un campo llamado `Referencia1`.
2. El **Backend AWS** recibe este campo y lo procesa.
3. Cuando el backend se conecta con el sistema **Postilion**, el campo se llama `NumeroCelular`.

---

## Mapeo de campos

| Origen       | Campo       | Destino      | Campo          | Notas                      |
|--------------|-------------|--------------|----------------|----------------------------|
| App móvil    | Referencia1 | Backend AWS  | Referencia1    | Campo enviado tal cual     |
| Backend AWS  | Referencia1 | Postilion    | NumeroCelular  | Campo renombrado para Postilion |

---

## Detalles adicionales

- La transformación del campo ocurre en la capa del backend AWS.
- Es importante validar que ambos campos representen el mismo dato semántico.
- En caso de que cambie el nombre en otros sistemas, esta tabla debe actualizarse.

---

## Diagramas

Se recomienda incluir diagramas para visualizar el flujo de datos.

