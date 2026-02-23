---
sidebar_position: 1
sidebar_label: 'Requerimientos'
---

# Requerimientos del Sistema de Inicio de Sesión Centralizado SSO
Ministerio de Economía

---

## 1. Requerimientos Funcionales

Los requerimientos funcionales definen las funcionalidades que debe cumplir el SSO para soportar la autenticación centralizada de todos los sistemas internos.

### RF01 — Autenticación de Usuarios
- Permitir que los usuarios inicien sesión utilizando credenciales almacenadas en LDAP.
- Validar usuario y contraseña contra el directorio central.
- Emitir token JWT para acceso a sistemas integrados.

### RF02 — Gestión de Roles y Permisos
- Definir y asignar roles a los usuarios.
- Mapear roles
- Permitir auditoría de cambios en roles y permisos.

### RF03 — Registro y Administración de Sistemas Clientes
- Registrar nuevos sistemas que usarán el SSO.
- Generar nuevo registro para cada sistema.

### RF04 — Logout Global
- Permitir que el usuario cierre sesión en todos los sistemas integrados desde el SSO.
- Invalidar tokens activos asociados al usuario.

### RF05 — Auditoría
- Mantener logs para auditorías internas y cumplimiento normativo.

---

## 2. Requerimientos No Funcionales

Los requerimientos no funcionales definen las características de calidad, rendimiento y seguridad que el sistema debe cumplir.

### RNF01 — Disponibilidad
- El sistema debe garantizar disponibilidad ≥ 99.9% en producción.

### RNF02 — Rendimiento
- Tiempo de respuesta de autenticación < 500 ms promedio.
- Soporte para múltiples solicitudes concurrentes sin degradación del servicio.

### RNF03 — Escalabilidad
- Capacidad de escalar horizontalmente según demanda.
- Preparado para integración con nuevos sistemas sin cambios estructurales.

### RNF04 — Seguridad
- Autenticación segura a través de LDAP.
- Transmisión cifrada.
- Tokens JWT.
- Protección.

### RNF05 — Mantenibilidad
- Código modular y documentado.
- Facilidad para actualizar configuraciones de LDAP y sistemas clientes.