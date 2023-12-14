# Endpoint: `GET /eventos/{id}`

Permite obtener información detallada sobre un evento específico mediante su identificador único.

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del tema que se desea recuperar.

## Ejemplo de Solicitud
```http
GET api/eventos/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "fecha": "2023-03-05",
            "evento": "Conferencia de Innovacion Tecnologica",
            "ubicacion": "Centro de Convenciones",
            "hora_inicio": "10:00:00.000",
            "hora_cierre": "13:00:00.000",
            "createdAt": "2023-12-09T07:47:07.571Z",
            "updatedAt": "2023-12-09T07:47:52.791Z",
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

- Asegurate de incluir un ID válido en la solicitud para obtener la información
  sobre un evento en específico.