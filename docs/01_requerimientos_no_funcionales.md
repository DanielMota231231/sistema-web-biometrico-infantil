# Requerimientos No Funcionales  
Sistema Web Biométrico Infantil

## Introducción
Este documento describe los requerimientos no funcionales del Sistema Web Biométrico Infantil.  
Estos requerimientos definen las condiciones de operación, seguridad, acceso, control y preparación del sistema antes de iniciar los sprints de desarrollo funcional.

---

## RNF-01 Control de versiones
**Descripción:**  
El sistema debe mantenerse bajo control de versiones para asegurar la trazabilidad de los cambios y el trabajo colaborativo.

**Criterios de aceptación:**
- El proyecto cuenta con un repositorio en GitHub.
- Se realizan commits incrementales con mensajes descriptivos.
- Se excluyen archivos locales y de configuración del entorno mediante `.gitignore`.

---

## RNF-02 Entorno de desarrollo
**Descripción:**  
El sistema debe poder ejecutarse en diferentes equipos de desarrollo de forma estandarizada.

**Criterios de aceptación:**
- El proyecto utiliza Python y el framework Django.
- Se emplea un entorno virtual para el manejo de dependencias.
- El repositorio contiene la estructura base del proyecto.

---

## RNF-03 Seguridad y control de acceso
**Descripción:**  
El sistema debe restringir el acceso únicamente a usuarios autenticados.

**Criterios de aceptación:**
- Existe una pantalla de inicio de sesión accesible desde `/login/`.
- Las rutas protegidas requieren autenticación previa.
- El punto de entrada principal del sistema redirige automáticamente al login.
- Se utiliza el sistema de autenticación integrado de Django.

---

## RNF-04 Roles de usuario
**Descripción:**  
El sistema contará con diferentes roles de usuario para definir niveles de acceso y responsabilidades.

**Roles definidos:**
- **Administrador:** Acceso total al sistema y configuración general.
- **Recepción:** Registro y consulta de información básica.
- **Asistente educativa:** Consulta y registro de actividades del menor.
- **Área médica/psicología:** Consulta y registro de información clínica.
- **Tutor:** Consulta de información relacionada exclusivamente a su hijo(a).

**Nota:**  
La implementación detallada de permisos por rol se realizará durante los sprints de desarrollo.

---

## RNF-05 Usabilidad
**Descripción:**  
El sistema debe ser fácil de usar y accesible desde un navegador web.

**Criterios de aceptación:**
- La interfaz presenta formularios claros y comprensibles.
- El acceso inicial al sistema es directo al inicio de sesión.
- La navegación es sencilla y sin pasos innecesarios.

---

## RNF-06 Preparación para procesos de ingreso
**Descripción:**  
El sistema debe contar con un formulario base para la captura de información de solicitudes de ingreso.

**Criterios de aceptación:**
- Existe un formulario de solicitud de ingreso para capturar información general del menor y del tutor.
- El formulario funciona como base de captura sin lógica de negocio.
- El procesamiento completo de la solicitud se implementará en fases posteriores.

---

## RNF-07 Evidencias y documentación
**Descripción:**  
El avance del sistema debe quedar documentado y respaldado con evidencias.

**Criterios de aceptación:**
- Se cuenta con documentación técnica en formato Markdown.
- Existen capturas del login funcionando.
- Los avances se reflejan en el historial de commits del repositorio.

---

## Conclusión
Los requerimientos no funcionales aquí descritos permiten establecer una base sólida para el desarrollo del Sistema Web Biométrico Infantil, garantizando seguridad, control de acceso, estandarización del entorno y preparación para el desarrollo por sprints.
