# Endpoint: `DELETE /usuarios/{id}`

Permite eliminar un usuario mediante su identificador unico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea elimninar.

## Ejemplo de Solicitud
```http
DELETE api/usuario/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "correo": "jorge@gmail.com",
            "nombre": "jorge",
            "apellido": "Gomez",
            "edad": 16,
            "ocupacion": "Estudiante",
            "createdAt": "2023-12-09T07:49:54.440Z",
            "updatedAt": "2023-12-14T08:17:33.239Z",
            "publishedAt": "2023-12-09T07:51:57.856Z"
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

- Asegurate de incluir un ID válido en la solicitud para eliminar al usuario deseado.
