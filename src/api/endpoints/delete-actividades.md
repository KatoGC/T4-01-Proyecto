# Endpoint: `DELETE /actividades/{id}`

Permite eliminar una actividad mediante su identificador unico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE api/actividades/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "Actividad": "Sesion de Entrenamiento en Pensamiento Critico",
            "Descripcion": "Actividad interactiva en línea que abarca ejercicios de análisis, resolución de problemas y toma de decisiones para estimular el pensamiento crítico en jóvenes",
            "createdAt": "2023-12-09T07:44:24.226Z",
            "updatedAt": "2023-12-09T07:44:24.226Z",
            "publishedAt": "2023-12-09T07:45:16.085Z"
        }
    },
    "meta": {}
}
```

## Respuestas de Errores Posibles
- Código 404 Not Found:

```json
{
    "data": null,
    "error": {
        "status": 404,
        "name": "NotFoundError",
        "message": "Not Found",
        "details": {}
    }
}
```

## Notas Adicionales

- Asegurate de incluir un ID válido en la solicitud para eliminar la actividad deseada.
