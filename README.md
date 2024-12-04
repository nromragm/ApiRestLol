
# API REST Lol

## Descripción

Una api rest donde los usuarios podran consultar y gestionar informacion sobre campeones partidas etc...

---

## Estructura de las entidades

Se trabajará con las siguientes tres entidades:

1. **Usuario**:
    - `id` (Long): Identificador único del usuario.
    - `username` (String): Nombre del usuario (debe ser único).
    - `password` (String): Contraseña del usuario (debe estar hasheada).
    - `rol` (String): Rol del usuario, que puede ser `USER` o `ADMIN`.

   
2. **Campeon**:
    - `id` (Long): Identificador único del campeón.
    - `nombre` (String): Nombre del campeón.
    - `tipo` (String): Tipo de campeón (asesino, mago, bruiser...).

3. **Partida**:
    - `id` (Long): Identificador único de la partida.
    - `fecha` (DateTime): Fecha y hora en que se jugó la partida.
    - `resultado` (String): Resultado de la partida (victoria, derrota).
    - `usuario_id` (Long): Identificador del usuario que participó en la partida (relación con la entidad **Usuario**).
    - `campeon_id` (Long): Identificador del campeón usado en la partida (relación con la entidad **Campeón**).
    - `duracion` (Integer): Duración de la partida en minutos.

---
