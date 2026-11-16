# Plan de pruebas funcionales

| Caso | Acción | Resultado esperado | Estado |
|---|---|---|---|
| P01 | Registro con rol admin enviado por cliente | Rol asignado: operario | Pendiente |
| P02 | Inicio de sesión incorrecto | HTTP 401 | Pendiente |
| P03 | Reportes sin token | HTTP 401 | Pendiente |
| P04 | Lote con vencimiento anterior a fabricación | Validación HTTP 400 | Pendiente |
| P05 | Crear lote con stock inicial | Inventario y movimiento coherentes | Pendiente |
| P06 | Salida válida | Descuenta existencias y registra historial | Pendiente |
| P07 | Salida superior al stock | Rechazo sin alterar inventario | Pendiente |
| P08 | Lote de otro producto | Rechazo sin alterar inventario | Pendiente |
| P09 | Exportación CSV | Encabezados y datos | Pendiente |
| P10 | Consulta de siete indicadores | Métricas coherentes | Pendiente |
| P11 | Exportación real de SQL Server | Importable en entorno aislado | Pendiente |

Adjuntar capturas de ejecución, fecha, resultado y observaciones de cada caso. No considerar pruebas pendientes como aprobadas.
