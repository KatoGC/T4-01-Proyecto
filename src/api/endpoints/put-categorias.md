# Endpoint: `PUT /categorias/{id}`

Permite actualizar parcialmente la información de una categoria específica mediante su identificador único.

## Parámetros de URL

- `{id}` (obligatorio): Identificador único de la categoria que se desea actualizar.

## Ejemplo de Solicitud

```json
PUT api/categorias/1
{
    "data":{
        "categoria":"Cognicion"
        }
}
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

- Asegurate de incluir un ID válido en la solicitud para actualizar la información sobre la categoria en específico.
- Recuerda que los campos que no se incluyan en la solicitud no serán actualizados.