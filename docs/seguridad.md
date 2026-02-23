# Seguridad
Ministerio de Economía

---

## 1. Gestión de Contraseñas

- Las **contraseñas de usuario** se gestionan exclusivamente en **LDAP**.  
- LDAP debe implementar **políticas de seguridad** como:
  - Complejidad mínima de contraseña.  
  - Expiración periódica.  
  - Bloqueo temporal por intentos fallidos.  

> El SSO no almacena contraseñas, sino que valida credenciales directamente contra LDAP.

---

## 2. Tokens de Autenticación

- El SSO emite **tokens JWT** firmados para cada sesión autenticada.  
- Los tokens tienen:
  - Expiración definida (por ejemplo, 15 minutos).  
  - Validación de firma en sistema integrado.  
  - Posibilidad de **revocación** mediante logout global.  

---

<!-- ## 3. Protección de la Comunicación

- Todas las comunicaciones deben realizarse a través de **HTTPS**.  
- Protección contra ataques comunes:
  - **CSRF** en formularios de autenticación.  
  - **XSS** en paneles administrativos.  
  - **Brute-force** mediante rate limiting en intentos de login.  

--- -->

## 3. Auditoría y Cumplimiento

- Registro de accesos exitosos y fallidos en la **bitácora del SSO**.  
- Monitoreo de cambios en roles y sistemas integrados.  
- Cumplimiento de políticas internas de seguridad.  
- Disponibilidad de logs para auditorías internas y externas.

---

## 4. Principios de Seguridad

1. LDAP como única fuente de identidad.  
2. **Tokens JWT** para autenticación segura entre sistemas.  
3. **Transmisión cifrada y validación constante** de accesos.  
4. **Auditoría completa** para cumplir normativa y trazabilidad.  