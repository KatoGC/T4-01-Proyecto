# Endpoint: `PUT /actividades/{id}`

Permite actualizar parcialmente la información de una actividad específico mediante su identificador único.

## Parámetros de URL

- `{id}` (obligatorio): Identificador único de la actividad que se desea actualizar.

## Ejemplo de Solicitud

```json
PUT api/actividad/3
{
    "data":{
        "Actividad":"Debate Abierto: Temas de la actualidad"
        }
}
```

## Respuesta Exitosa (Código 200 OK)

```json
{
    "data": {
        "id": 3,
        "attributes": {
            "Actividad": "Debate Abierto: Temas de la actualidad",
            "Descripcion": "Foro virtual donde los participantes discuten y argumentan sobre temas actuales, promoviendo el análisis crítico y la argumentación lógica.",
            "createdAt": "2023-12-09T07:44:49.613Z",
            "updatedAt": "2023-12-14T08:29:01.846Z",
            "publishedAt": "2023-12-09T07:45:16.085Z"
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

- Asegurate de incluir un ID válido en la solicitud para actualizar la información sobre la actividad en específico.
- Recuerda que los campos que no se incluyan en la solicitud no serán actualizados.