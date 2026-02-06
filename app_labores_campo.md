# App móvil para registro de labores de campo

## Objetivo
Crear una app móvil sencilla para registrar labores agrícolas en campo, con énfasis en rapidez de captura y funcionamiento offline.

## Funcionalidades clave
- **Registro de labor**: tipo de labor, cultivo/lote, fecha, hora de inicio/fin, personal, maquinaria, insumos y observaciones.
- **Gestión de lotes/cultivos**: catálogo de lotes, cultivos y superficies.
- **Personal y cuadrillas**: alta de trabajadores, roles y asignaciones.
- **Insumos**: catálogo y consumo por labor.
- **Adjuntos**: fotos y notas de voz por labor.
- **Geolocalización**: ubicación opcional del registro.
- **Modo offline**: guardar localmente y sincronizar cuando haya conexión.
- **Reportes**: resumen por lote, por labor, por periodo y por trabajador.

## Campos mínimos sugeridos
- Lote
- Cultivo
- Tipo de labor
- Fecha
- Hora de inicio y fin
- Personal / cuadrilla
- Observaciones

## Flujo propuesto
1. Seleccionar lote y cultivo.
2. Elegir tipo de labor.
3. Completar tiempos, personal y notas.
4. Adjuntar fotos (opcional) y ubicación (opcional).
5. Guardar (sincronizar si hay conexión).

## Consideraciones técnicas
- **Plataforma**: Android inicialmente (más común en campo), con posibilidad de iOS.
- **Persistencia local**: base de datos local (SQLite/Room).
- **Sincronización**: API REST y colas de sincronización.
- **Seguridad**: autenticación por usuario y permisos por rol.

## Próximos pasos
- Validar campos obligatorios con usuarios.
- Priorizar laboratorios más frecuentes.
- Definir backend y esquema de datos.
