# Endpoint: `POST /usuarios`

Permite añadir un nuevo usuario a la coleccion de usuarios.

## Ejemplo de Solicitud
```json
POST api/usuario

{
    "data": {
        "correo": "ejemplo@example.com",
        "nombre": "ejemplo",
        "apellido": "test",
        "edad": "19",
        "ocupacion": "ejemplo"
    }
}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 5,
        "attributes": {
            "correo": "ejemplo@example.com",
            "nombre": "ejemplo",
            "apellido": "test",
            "edad": 19,
            "ocupacion": "ejemplo",
            "createdAt": "2023-12-14T07:54:51.139Z",
            "updatedAt": "2023-12-14T07:54:51.139Z",
            "publishedAt": "2023-12-14T07:54:51.134Z"
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

- Asegurate de incluir los parametros adecuados para agregar el usuario.
