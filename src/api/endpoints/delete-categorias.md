# Endpoint: `DELETE /categorias/{id}`

Permite eliminar una categoria mediante su identificador unico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE api/categorias/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "categoria": "Cognicion",
            "createdAt": "2023-12-09T07:45:46.099Z",
            "updatedAt": "2023-12-14T08:31:14.259Z",
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

- Asegurate de incluir un ID válido en la solicitud para eliminar la categoria deseada.
