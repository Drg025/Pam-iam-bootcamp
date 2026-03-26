#  Zero to Hero: Privileged Access Management (PAM) Bootcamp

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-blue)
![Active Directory](https://img.shields.io/badge/Tech-Active%20Directory-blue)
![PowerShell](https://img.shields.io/badge/Scripting-PowerShell-5391FE)
![CyberArk](https://img.shields.io/badge/PAM-CyberArk-black)
![BeyondTrust](https://img.shields.io/badge/PAM-BeyondTrust-orange)

Bienvenido a mi repositorio. Este proyecto documenta un plan de estudio intensivo y autodidacta de 5 meses diseñado para dominar los fundamentos de la Gestión de Accesos Privilegiados (PAM), Identity & Access Management (IAM), y la automatización de infraestructura. 

El objetivo principal es pasar de conceptos teóricos a la capacidad operativa para administrar, asegurar y automatizar entornos empresariales críticos.

---

##  Objetivos del Bootcamp
- Comprender a fondo la arquitectura de **Identity & Access Management (IAM)** y el ciclo de vida de las identidades.
- Dominar **PowerShell** como herramienta principal para la automatización, gestión de Active Directory y consumo de APIs (REST).
- Entender la arquitectura, despliegue y administración de los líderes de la industria PAM: **CyberArk** y **BeyondTrust Password Safe**.
- Crear un entorno de laboratorio funcional para simular ataques, auditorías y rotación de credenciales.

---

##  Roadmap de 5 Meses

###  Mes 1: El Ecosistema de Identidad (Active Directory & IAM)
*El 90% de los problemas de PAM nacen en Active Directory.*
- **Semana 1:** Fundamentos IAM (AAA, RBAC, ABAC, JML - Joiner, Mover, Leaver).
- **Semana 2:** Instalación de Windows Server y configuración de Domain Controller (DC) en laboratorio virtual.
- **Semana 3:** Gestión profunda de Usuarios, Grupos de Seguridad y Unidades Organizativas (OU).
- **Semana 4:** Protocolos de autenticación: Kerberos, NTLM, LDAP y DNS.

###  Mes 2: PowerShell - De Scripting a Automatización
*La herramienta indispensable para gestionar a escala.*
- **Semana 1:** Sintaxis base, Variables, Objetos y dominio del Pipeline (`|`).
- **Semana 2:** Módulo de Active Directory (`Get-ADUser`, `New-ADGroup`).
- **Semana 3:** Scripting avanzado: Funciones, manejo de errores (`Try/Catch`), bucles (`ForEach`).
- **Semana 4:** Módulo `SecretManagement` y APIs REST (Conectando PowerShell con herramientas web sin credenciales en texto plano).

###  Mes 3: Inmersión en CyberArk
*Comprendiendo el estándar de la industria.*
- **Semana 1:** Teoría PAM (Riesgos, Compliance, Auditoría) e Introducción a CyberArk.
- **Semana 2:** Arquitectura CyberArk: Digital Vault, CPM, PSM, PVWA, y Disaster Recovery.
- **Semana 3:** Operación diaria: Onboarding de cuentas, Safes, Master Policy, Platform Management.
- **Semana 4:** Credential Providers (CP) y eliminación de credenciales hardcodeadas (AAM).
- **Hito:** Obtención de la certificación gratuita *CyberArk Trustee*.

###  Mes 4: BeyondTrust & Operaciones de Seguridad
*Conociendo alternativas y procesos operativos.*
- **Semana 1:** Arquitectura BeyondTrust Password Safe (U-Series, BeyondInsight).
- **Semana 2:** Smart Rules y Discovery (Automatización de hallazgo de cuentas huérfanas).
- **Semana 3:** Gestión de Sesiones (RDP/SSH Proxy), Auditoría y Endpoint Privilege Management.
- **Semana 4:** Comparativa Técnica y de Casos de Uso: CyberArk vs. BeyondTrust.

###  Mes 5: Nube, Integraciones y Proyecto Final
*Llevando la identidad al entorno híbrido.*
- **Semana 1:** Microsoft Entra ID (Azure AD) y Privileged Identity Management (PIM).
- **Semana 2:** Integraciones teóricas de PAM con herramientas de ticketing (ServiceNow) y SIEMs (Splunk/Sentinel).
- **Semana 3 & 4:** **Proyecto Final (Capstone):** Diseño arquitectónico y scripting para un escenario empresarial simulado (Migración masiva y automatización de Onboarding).

---

##  Herramientas y Laboratorio
- **Virtualización:** Oracle VirtualBox / VMware Workstation.
- **Sistemas Operativos:** Windows Server 2019/2022, Windows 10/11 Enterprise, distribuciones Linux base.
- **Editor:** Visual Studio Code (con extensiones de PowerShell y Markdown).
- **Control de Versiones:** Git & GitHub.

---

##  Consejos

1. **Sincronización Total:** Mantén tus apuntes, diagramas y scripts de PowerShell sincronizados entre tu PC de escritorio y tu laptop usando herramientas como Syncthing. Tener tus notas a la mano en cualquier dispositivo te salvará la vida cuando estés haciendo *troubleshooting* de Active Directory o repasando conceptos.
2. **El Laboratorio es tu Mejor Amigo:** No te quedes solo viendo tutoriales en YouTube. Levanta las máquinas virtuales, rompe el Active Directory y vuélvelo a arreglar. La experiencia real viene de leer los logs de error.
3. **Documenta los Errores:** Cada vez que un script de PowerShell falle o un GPO no se aplique, anota el código de error y cómo lo solucionaste. Este repositorio debe convertirse en tu propia base de conocimiento.
4. **Cuidado con los Secretos:** Nunca subas scripts a este repositorio que contengan contraseñas reales, IPs públicas o datos sensibles. Usa variables de entorno o módulos de gestión de secretos.
5. **Dibuja la Arquitectura:** Las herramientas PAM son abstractas. Dibuja diagramas de flujo de cómo viaja una contraseña desde que un usuario la solicita hasta que se inyecta en el servidor destino.
6. **Errores y Troubleshooting** Esta es la sección más valiosa para un ingeniero. ¿Qué se rompió y cómo lo arreglaste?.
Error encontrado: [Ej. El script me dio un error de "Access Denied" al ejecutar Invoke-Command]
Causa raíz: [Ej. No estaba ejecutando la consola como Administrador / Faltaba habilitar WinRM]
Solución aplicada: [Ej. Ejecutar Enable-PSRemoting -Force en el servidor destino]

---
> *"La identidad es el nuevo perímetro de seguridad."*
