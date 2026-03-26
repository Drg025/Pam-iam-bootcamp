# Directorio de Recursos: PAM, IAM y Automatización

Bienvenido a mi directorio de estudio. Armé este documento para centralizar toda la bibliografía, herramientas y documentación técnica que estoy usando en mi camino para dominar la Gestión de Accesos Privilegiados (PAM), la automatización de infraestructura y Active Directory.

---

## 1. Active Directory y Fundamentos IAM
La base de la identidad corporativa. Si no entendemos cómo funciona un dominio por debajo, es imposible asegurarlo correctamente.

### Conceptos Core y Laboratorio
* **Laboratorio Práctico:** [TryHackMe - Active Directory Basics](https://tryhackme.com/room/activedirectorybasics). Es un excelente punto de partida para explorar un entorno real virtualizado, y de paso ayuda bastante a agarrar agilidad si también te interesan los CTFs.
* **Video Maestro:** [Active Directory Masterclass](https://www.youtube.com/results?search_query=Active+Directory+Masterclass+John+Savill) por John Savill. Dura unas 3 horas, pero explica el panorama completo desde cero.

### Protocolos de Autenticación
* **Lectura Oficial:** [Cómo funciona el protocolo Kerberos](https://learn.microsoft.com/es-es/windows-server/security/kerberos/how-the-kerberos-version-5-authentication-protocol-works) en la documentación de Microsoft.
* **Explicación Visual:** [Kerberos Authentication Explained](https://www.youtube.com/results?search_query=Kerberos+Authentication+Explained+HackerSploit) por HackerSploit.
* **Control de Accesos:** [RBAC vs ABAC - Access Control Models](https://www.youtube.com/results?search_query=RBAC+vs+ABAC+Inside+Cloud+and+Security).

---

## 2. PowerShell y Automatización
Mi herramienta principal para no tener que hacer tareas repetitivas a mano y poder gestionar todo a escala.

### Fundamentos y Scripting Avanzado
* **El Libro de Cabecera:** Learn Windows PowerShell in a Month of Lunches. Es el estándar para aprender scripting administrativo.
* **Ruta Práctica:** [Automatización de tareas con PowerShell](https://learn.microsoft.com/es-es/training/paths/windows-powershell-basics/) de Microsoft Learn.
* **Para Escuchar:** The PowerShell Podcast. Muy bueno para escuchar casos de uso reales de automatización.

### Gestión de Secretos
* **Documentación:** [Módulo Microsoft.PowerShell.SecretManagement](https://learn.microsoft.com/es-es/powershell/module/microsoft.powershell.secretmanagement/). Crucial para no dejar contraseñas en texto plano en los scripts.
* **Demostración:** [SecretManagement Module Overview](https://www.youtube.com/results?search_query=PowerShell+SecretManagement+Module+Overview).

---

## 3. CyberArk (Privileged Access Security)
El estándar actual de la industria para PAM. Como es difícil conseguir licencias para practicar en casa, me enfoco mucho en entender su arquitectura teórica.

### Arquitectura y Certificación Base
* **Certificación Oficial (Gratuita):** [CyberArk Trustee Certification](https://training.cyberark.com/learn). Solo requiere crear una cuenta en su universidad virtual.
* **Visión General:** [CyberArk Architecture and Component Overview](https://www.youtube.com/results?search_query=CyberArk+Architecture+and+Component+Overview+Online+Tech+Cloud).

### Operaciones y Automatización
* **Tutoriales de Operación:** Lista de reproducción [CyberArk Tutorial for Beginners](https://www.youtube.com/results?search_query=CyberArk+Tutorial+for+Beginners+Online+Tech+Cloud). Muestra cómo operan el CPM y el PSM.
* **Código y API:** [Módulo psPAS en GitHub](https://pspas.pspete.dev/). Un módulo de la comunidad buenísimo para interactuar con CyberArk usando PowerShell.

---

## 4. BeyondTrust Password Safe
Una gran alternativa a CyberArk para entender diferentes formas de abordar el mismo problema de seguridad, especialmente su enfoque en quitar permisos locales.

### Consola y Operaciones
* **Demos Oficiales:** Lista [BeyondTrust Password Safe Demos](https://www.youtube.com/results?search_query=BeyondTrust+Password+Safe+Demos).
* **Conceptos:** Whitepapers de la BeyondTrust University.

### Endpoint Privilege Management (EPM)
* **Demostración:** [Endpoint Privilege Management Demo](https://www.youtube.com/results?search_query=BeyondTrust+Endpoint+Privilege+Management+Demo). Muestra cómo un usuario estándar puede operar sin necesitar la contraseña de administrador local.

---

## 5. IAM en la Nube
Llevando la identidad fuera de la red local.

* **Video Maestro:** [Microsoft Entra ID Masterclass](https://www.youtube.com/results?search_query=Microsoft+Entra+ID+Masterclass+John+Savill) por John Savill.
* **Ruta de Aprendizaje:** [SC-300: Implementación de la administración de identidades](https://learn.microsoft.com/es-es/training/paths/implement-identity-management-azure-ad/).
* **Lectura:** [What is Just-in-Time Access?](https://www.cyberark.com/what-is/just-in-time-access/) por CyberArk.

---

## Notas sobre mi entorno de Laboratorio y Apuntes

Para no consumir todos los recursos de mi computadora principal, configuré un mini PC como mi servidor personal. Ahí levanto mis máquinas virtuales de Windows Server, y utilizo mi entorno Linux del día a día para administrar todo de forma remota. Lo recomiendo bastante porque simula un escenario empresarial mucho más realista.

Por otro lado, mantengo toda la documentación de este proceso organizada en Obsidian. Me resulta la mejor manera de ir enlazando los conceptos teóricos de gestión de identidades directamente con los scripts de PowerShell que voy armando.