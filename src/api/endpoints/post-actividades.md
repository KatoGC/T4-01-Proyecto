# Endpoint: `POST /actividades`

Permite añadir un nueva actividad a la coleccion de actividades.

## Ejemplo de Solicitud
```json
POST api/actividades

{
    "data":{
        "Actividad": "Debate Abierto: IA",
        "Descripcion": "Actividad interactiva en línea que abarca ejercicios de análisis respecto a las Inteligencias Artificiales"
        }
}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 6,
        "attributes": {
            "Actividad": "Debate Abierto: IA",
            "Descripcion": "Actividad interactiva en línea que abarca ejercicios de análisis respecto a las Inteligencias Artificiales",
            "createdAt": "2023-12-14T08:09:07.078Z",
            "updatedAt": "2023-12-14T08:09:07.078Z",
            "publishedAt": "2023-12-14T08:09:07.075Z"
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

- Asegurate de incluir los parametros adecuados para agregar la actividades.