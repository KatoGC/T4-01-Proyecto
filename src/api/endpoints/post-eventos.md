# Endpoint: `POST /eventos`

Permite añadir un nuevo evento a la coleccion de evento.

## Ejemplo de Solicitud
```json
POST /eventos

{
    "data":{
        "fecha": "2023-07-12",
        "evento": "Conferencia de Redes Neuronales",
        "ubicacion": "Centro de Tecnologia",
        "hora_inicio": "12:00:00.000",
        "hora_cierre": "17:00:00.000"
        }
}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 5,
        "attributes": {
            "fecha": "2023-07-12",
            "evento": "Conferencia de Redes Neuronales",
            "ubicacion": "Centro de Tecnologia",
            "hora_inicio": "12:00:00.000",
            "hora_cierre": "17:00:00.000",
            "createdAt": "2023-12-14T08:01:35.287Z",
            "updatedAt": "2023-12-14T08:01:35.287Z",
            "publishedAt": "2023-12-14T08:01:35.285Z"
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

- Asegurate de incluir los parametros adecuados para agregar el evento.