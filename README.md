# Base-de-Datos-de-Cuerpos-Celestiales-
Base de datos relacional en PostgreSQL con galaxias, estrellas, planetas, lunas y asteroides. Proyecto de freeCodeCamp con claves primarias, foráneas y relaciones entre tablas.
# Base de Datos de Cuerpos Celestiales

Proyecto del curso Relational Database de freeCodeCamp. Es una base de datos en PostgreSQL con galaxias, estrellas, planetas, lunas y asteroides.

## Tablas

- `galaxy`: galaxias
- `star`: estrellas, cada una pertenece a una galaxia
- `planet`: planetas, cada uno orbita una estrella
- `moon`: lunas, cada una orbita un planeta
- `asteroid`: asteroides

## Qué aprendí

- Crear tablas con claves primarias y foráneas
- Relacionar tablas entre sí (galaxia → estrella → planeta → luna)
- Usar restricciones como `UNIQUE` y `NOT NULL`
- Insertar datos con `INSERT INTO`
- Consultar columnas y filas con `SELECT`
- Exportar y restaurar una base de datos con `pg_dump` y `psql`

## Cómo usarla

```bash
psql -U postgres < universe.sql
```

Ejemplo para consultar datos:

```sql
SELECT name, star_type FROM star;
```

Algunos datos son inventados, solo sirven para practicar.
