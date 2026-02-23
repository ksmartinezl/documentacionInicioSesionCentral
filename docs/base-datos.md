# Modelo de Datos
Ministerio de Economía

---

## 1. LDAP

El LDAP actúa como directorio central de usuarios, almacenando las credenciales y atributos esenciales de cada usuario.  

### Entidades LDAP
- **users:** Usuarios del Ministerio con credenciales y atributos básicos.
- **atributos de usuario:** Campos como `email`, `estado`, `nombre`, `grupo` (para mapear roles internos).


---

## 2. Base de Datos del SSO

La base de datos del SSO se encarga de gestionar la información adicional que no se encuentra en LDAP, incluyendo roles, sistemas integrados y auditoría.

### Entidades Principales

| Entidad             | Descripción |
|--------------------|-------------|
| **Roles**           | Define los roles internos del SSO (ej. Administrador, Usuario, Auditor). |
| **Usuarios**        | Usuarios registrados en el SSO, referenciando LDAP. |
| **Roles de Sistema**| Relación entre roles y sistemas específicos. |
| **Sistemas**        | Sistemas clientes integrados al SSO|
| **Accesos**         | Relación entre roles y usuarios específicos. |
| **Bitácora**        | Logs de inicio de sesión. |

---

## 3. Diseño de Base de Datos

A continuación se muestra el **modelo visual de la base de datos**, incluyendo la relación entre LDAP y la base del SSO:

![Modelo de Base de Datos](./images/db.png)
