# 📅 Día [X]: [Título Principal del Tema]
**Fecha:** DD/MM/AAAA  
**Módulo:** [Ej. Mes 1 - Active Directory / Mes 2 - PowerShell]  
**Tiempo invertido:** [Ej. 2 horas]

---

## 🧠 Conceptos Clave Aprendidos
*Anota aquí la teoría pura en viñetas cortas.*
* **Concepto 1:** Definición o explicación breve.
* **Concepto 2:** Cómo se relaciona con IAM/PAM.
* **Concepto 3:** Notas adicionales.

## 💻 Práctica y Comandos (Laboratorio)
*Documenta los scripts o comandos que ejecutaste hoy. Usa bloques de código.*

**Objetivo del script/comando:** [Ej. Crear 5 usuarios de prueba en AD]

```powershell
# Escribe tu código aquí
$users = Import-Csv -Path "C:\temp\users.csv"
foreach ($user in $users) {
    Write-Host "Creando usuario: $($user.Name)"
}