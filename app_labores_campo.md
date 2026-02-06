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

## Cómo usarla (flujo simple)
1. **Configurar catálogos**: cargar lotes, cultivos, personal e insumos una sola vez.
2. **Crear una labor**: seleccionar lote y cultivo, luego elegir el tipo de labor.
3. **Completar el registro**: ingresar tiempos, personal, insumos y observaciones.
4. **Adjuntar evidencia**: agregar fotos, notas de voz y ubicación si aplica.
5. **Guardar y sincronizar**: guardar localmente y sincronizar al tener internet.
6. **Consultar reportes**: filtrar por lote, labor, periodo o trabajador.

## Cómo probarla en el celular
> **Nota**: este documento define la idea y los requisitos. Aún no existe una app funcional en este repositorio.

Para poder abrirla en tu celular necesitas primero un **prototipo** o un **MVP** (app mínima viable). Opciones rápidas:
- **Prototipo navegable**: diseñar en Figma y probar el flujo sin código.
- **MVP móvil**: construir una app simple (por ejemplo con Flutter o React Native) para capturar y guardar labores.

Cuando exista el MVP, la forma típica de probarlo es:
1. **Instalar el entorno de desarrollo** (Flutter/React Native según se elija).
2. **Ejecutar la app en modo desarrollo** y abrirla en el celular (por cable o con QR).
3. **Probar el flujo** de registro, adjuntos y sincronización offline.

## Consideraciones técnicas
- **Plataforma**: Android inicialmente (más común en campo), con posibilidad de iOS.
- **Persistencia local**: base de datos local (SQLite/Room).
- **Sincronización**: API REST y colas de sincronización.
- **Seguridad**: autenticación por usuario y permisos por rol.

## Próximos pasos
- Validar campos obligatorios con usuarios.
- Priorizar labores más frecuentes.
- Definir backend y esquema de datos.
