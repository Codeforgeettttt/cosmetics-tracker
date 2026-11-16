# Configurar el primer administrador

1. Crea la base nueva con backend/database/schema.sql.
2. Registra una cuenta normalmente: el rol inicial debe ser operario.
3. En SQL Server identifica la cuenta exacta: `SELECT id, nombre, email, rol_id FROM usuarios;`
4. En una base propia y autorizada, ejecuta:

```sql
UPDATE usuarios
SET rol_id = (SELECT id FROM roles WHERE nombre = 'admin')
WHERE email = 'CAMBIAR_POR_CORREO_DEL_ADMIN';
```

5. Cierra sesión y vuelve a ingresar para recibir un token con el rol actualizado.

Nunca permitas indicar `rol_id` desde el registro público.
