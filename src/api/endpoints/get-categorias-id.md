# Endpoint: `GET /categorias/{id}`

Permite obtener información detallada sobre una categoria específica mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea recuperar.

## Ejemplo de Solicitud
```http
GET api/categorias/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "categoria": "Deportes",
            "createdAt": "2023-12-09T07:45:46.099Z",
            "updatedAt": "2023-12-09T07:45:46.099Z",
            "publishedAt": "2023-12-09T07:46:31.596Z"
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

- Asegurate de incluir un ID válido en la solicitud para obtener la información
  sobre una categoria en específica.