
# Contexto y Justificación
Ministerio de Economía

---

## 1. Contexto General

Actualmente, los sistemas internos del Ministerio de Economía manejan **credenciales independientes**, lo que genera varios problemas:

- Los usuarios deben recordar múltiples credenciales.
- La trazabilidad de accesos es limitada.
- La seguridad global del acceso a los sistemas internos es inconsistente.
- La integración de nuevos sistemas es compleja y propensa a errores.

El **SSO centralizado con LDAP** permitirá resolver estos problemas al ofrecer una **fuente única de identidad** para todos los sistemas internos.

---

## 2. Problema a Resolver

1. **Gestión dispersa de usuarios:** Cada sistema administra credenciales propias.  
2. **Falta de trazabilidad y auditoría:** Difícil seguimiento de accesos y cambios.  
3. **Riesgos de seguridad:** Mayor probabilidad de contraseñas débiles o repetidas.  
4. **Integración compleja:** Cada sistema requiere configuración independiente de autenticación.

---

## 3. Justificación del Proyecto

- **Centralización de usuarios:** LDAP como directorio único para todos los sistemas.  
- **Seguridad y cumplimiento:** Accesos controlados y auditables, cumpliendo políticas institucionales.  
- **Eficiencia operativa:** Reducción de incidencias relacionadas con contraseñas y accesos.  
- **Escalabilidad:** Facilidad para integrar nuevos sistemas internos sin modificar la arquitectura central.  

---

## 4. Stakeholders Principales

- **Dirección TI:** Definición de políticas y supervisión.  
- **Equipos de Desarrollo:** Integración de sistemas con el SSO.  
- **Auditoría Interna:** Revisión de logs y cumplimiento normativo.