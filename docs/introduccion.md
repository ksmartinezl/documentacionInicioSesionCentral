---
sidebar_label: 'Introducción'
---

# Sistema de Inicio de Sesión Centralizado (SSO)
Ministerio de Economía

---

## 1. Descripción General

El **Sistema de Inicio de Sesión Centralizado (SSO)** tiene como objetivo principal **unificar la autenticación de todos los sistemas internos del Ministerio de Economía**, utilizando **LDAP como directorio de usuarios**. Esto permitirá:

- Centralizar la gestión de credenciales y roles.
- Mejorar la seguridad y trazabilidad de accesos.
- Facilitar la integración de nuevos sistemas internos.
- Proporcionar auditoría completa para cumplimiento normativo.

---

## 2. Objetivos del Sistema

### Objetivo General
Implementar un **proveedor de identidad institucional (IdP)** que autentique usuarios y emita **tokens seguros (JWT)** para todos los sistemas integrados.

### Objetivos Específicos
- Garantizar autenticación confiable mediante LDAP.
- Proveer un mecanismo de **logout global**.
- Gestionar roles y permisos centralizados.
- Registrar y auditar eventos críticos de acceso.
- Facilitar la integración de nuevos sistemas de manera estandarizada.

---

## 3. Alcance del Proyecto

### Incluye
- Autenticación de usuarios con LDAP.
- Administración de roles y permisos.
- Registro y configuración de sistemas clientes.
- Auditoría de accesos y cambios.
- Logout centralizado.

### No Incluye
- MFA u otros factores de autenticación adicionales.
- Sistemas externos no integrados al Ministerio.
- Funcionalidades de gestión de identidad fuera del dominio del SSO.

---

## 4. Beneficios Esperados
- Reducción de credenciales duplicadas y riesgo de seguridad.
- Mejor experiencia para usuarios internos.
- Cumplimiento con políticas institucionales de TI.
- Base sólida para futuras integraciones y mejoras.