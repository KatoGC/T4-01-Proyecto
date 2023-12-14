# Endpoint: `POST /categorias`

Permite añadir un nueva categoria a la coleccion de categoria.

## Ejemplo de Solicitud
```json
POST /categorias

{
    "data":{
        "categoria":"Mecanografia"
        }
}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 6,
        "attributes": {
            "categoria": "Mecanografia",
            "createdAt": "2023-12-14T08:04:52.233Z",
            "updatedAt": "2023-12-14T08:04:52.233Z",
            "publishedAt": "2023-12-14T08:04:52.231Z"
        }
    },
    "meta": {}
}
```

## Respuestas de Errores Posibles
- Código 400 Bad Request:

```json
{
    "data": null,
    "error": {
        "status": 400,
        "name": "ValidationError",
        "message": "Missing \"data\" payload in the request body",
        "details": {}
    }
}
```

## Notas Adicionales

- Asegurate de incluir los parametros adecuados para agregar la categoria.