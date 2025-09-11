# OCTAVE — “Mouse Jiggler” en equipo bancario

> **Nota:** Ejercicio **defensivo** de gestión de riesgo. No describe técnicas para evadir controles; su objetivo es evaluar y mitigar riesgos conforme a OCTAVE.

## Fase 1: Perfiles de amenazas basados en activos

### Activos críticos
- Sesión autenticada en PC/VDI corporativo  
- Datos de clientes/transacciones y credenciales (tokens, PIV)  
- Registros/auditoría (trazabilidad)

### Requisitos de seguridad
- **Confidencialidad / Integridad:** Alta  
- **Disponibilidad:** Media–Alta  
- **Trazabilidad y cumplimiento:** Críticos en banca

### Amenazas clave
- Empleado/contratista conecta “mouse jiggler” para evitar bloqueo
- Dispositivo HID compuesto (BadUSB + jiggler) inyecta comandos
- Sesiones VDI “pegadas” que permiten consultas/exfiltración sin supervisión

---

## Fase 2: Vulnerabilidades de infraestructura

### Tecnológicas
- Puertos **USB** habilitados sin *allow‑listing* de configs
- Bloqueo por inactividad basado solo en movimiento (sin re‑login)  
- Timeouts largos de aplicación/SSO

### Puntos de acceso
- USB frontales/docking stations.

### Prácticas actuales (suposiciones mínimas)
- Sin control de dispositivos (Device Control) a nivel endpoint  
- Alertas limitadas por nuevos HID/teclados

---

## Fase 3: Estrategia y planes

### Mitigación (básico)

**Preventivo**
- Device Control: **permitir solo HID aprobados** (allow‑list) y **bloquear dispositivos compuestos**
- MDM: re‑autenticación obligatoria al desbloquear; deshabilitar nuevos HID sin aprobación
- Timeouts de **aplicación/SSO** independientes del input
- Bloqueadores físicos de USB en áreas críticas; principio de menor privilegio
- Política explícita: **prohibición de jigglers/USB no autorizados**

**Detectivo**
- EDR/SIEM: alerta por **nuevo HID/teclado** o dispositivo compuesto
- UEBA: patrón de **ratón activo sin tecleo** prolongado

**Correctivo**
- Playbook “USB no autorizado”: aislar equipo, revocar sesiones/tokens, revisar logs

### Plan rápido (30/60/90)

- **0–30 días:** comunicar política; GPO re‑login obligatorio; port blockers en zonas clave  
- **31–60 días:** desplegar Device Control y endurecer timeouts de apps/SSO  
- **61–90 días:** revisar excepciones operativas y realizar auditoría de efectividad con revisión de logs.

### Métricas simples
- % endpoints con Device Control activo  
- # intentos USB bloqueados/mes  
- % equipos que cumplen re‑login/timeout

### Riesgo resumido
- **Probabilidad:** Media–Alta  
- **Impacto:** Alto (cumplimiento, reputación, datos)  
- **Nivel global:** **Alto/Crítico** si no hay Device Control + re‑login