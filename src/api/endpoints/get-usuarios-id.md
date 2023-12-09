# Endpoint: `GET /usuarios/{id}`

Permite obtener información detallada sobre un usuario específico mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /usuario/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "correo": "manuel@gmail.com",
    "nombre": "Manuel",
    "apellido": "Gomez",
    "edad": 16,
    "ocupacion": "Estudiante",
    "createdAt": "2023-12-09T07:49:54.440Z",
    "updatedAt": "2023-12-09T07:50:17.866Z",
    "publishedAt": "2023-12-09T07:51:57.856Z"
}
```

## Respuestas de Errores Posibles
- Código 404 Not Found:

  ```json
  {
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
  sobre un usuario en específico.
