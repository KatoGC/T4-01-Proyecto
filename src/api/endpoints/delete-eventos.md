# Endpoint: `DELETE /eventos/{id}`

Permite eliminar un evento mediante su identificador unico.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea eliminar.

## Ejemplo de Solicitud
```http
DELETE api/eventos/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "fecha": "2023-03-05",
            "evento": "Conferencia de Innovacion Tecnologica",
            "ubicacion": "Auditorio central",
            "hora_inicio": "10:00:00.000",
            "hora_cierre": "13:00:00.000",
            "createdAt": "2023-12-09T07:47:07.571Z",
            "updatedAt": "2023-12-14T08:32:40.363Z",
            "publishedAt": "2023-12-09T07:52:04.274Z"
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

- Asegurate de incluir un ID válido en la solicitud para eliminar el evento deseada.
