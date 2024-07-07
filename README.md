Desafío 17 – Miriam Romitelli.
Desarrollo de un Sistema de Gestión de Seguridad de la Información (SGSI) para una organización que aloja aplicaciones en la nube, y aplicar el ciclo PDCA con enfoque en dos aspectos de seguridad (Identificación y Autenticación, y Autorización) en un entorno Linux (sistema operativo + servidor web + base de datos).
Programa completo: 
Objeto de estudio: Sistema Operativo Linux (Ubuntu) + Servidor Web (Apache) + Base de Datos (MySQL).
Aspecto de Seguridad: Identificación y Autenticación
Objetivo 1: Mejorar la Gestión de Identidades y Autenticación
Planificar:
1.	Identificar todos los sistemas y recursos críticos que requieren autenticación.
Servidor Web (Apache):
•	Identificar los sitios web y aplicaciones alojadas en el servidor Apache.
•	Determinar si se requiere autenticación para el acceso a la administración del servidor o a las aplicaciones específicas.
Base de Datos (MySQL):
•	Listar las bases de datos críticas que almacenan información sensible.
•	Definir los usuarios y privilegios necesarios para cada base de datos según los roles de usuario (por ejemplo, administrador, desarrollador, usuario final).
Sistema Operativo (Linux):
•	Identificar los usuarios con acceso administrativo (root) y asegurarse de que la autenticación para estos usuarios sea robusta (por ejemplo, mediante MFA si es posible).
2.	Definir políticas claras de creación, gestión y eliminación de cuentas de usuario.
Requisitos de Creación:
Establecer criterios claros para la creación de nuevas cuentas de usuario. Por ejemplo, podría requerir que todas las solicitudes de creación de cuentas sean aprobadas por un administrador de sistemas o por un supervisor.
Información: Definir qué información debe proporcionar un usuario al solicitar una cuenta (nombre completo, departamento, motivo de acceso, etc.).
Políticas de Contraseñas: Especificar los requisitos.
Ejemplo Práctico:
Las contraseñas deben tener al menos 10 caracteres de longitud.
Deben incluir al menos un carácter especial y un número.
Las contraseñas deben cambiarse cada 90 días.
No se pueden reutilizar las últimas cinco contraseñas.
Auditorías y Revisiones: Establecer procedimientos regulares para revisar y auditar las cuentas de usuario para garantizar que estén activas y sean necesarias.
Ejemplo Práctico - Suspensión y Reactivación:
Las cuentas de usuario serán suspendidas automáticamente después de 7 días de inactividad.
Las cuentas suspendidas se pueden reactivar dentro de los 30 días posteriores a la suspensión, previa solicitud del supervisor del usuario y aprobación del administrador de sistemas.
Políticas de Eliminación de Cuentas de Usuario
El administrador de sistemas eliminará la cuenta de usuario y revocará todos los accesos y privilegios asociados.
Implementación
Una vez que se haya definido estas políticas, es fundamental comunicarlas claramente a todos los empleados relevantes y asegurarse de que se implementen de manera efectiva y se mantengan actualizadas a medida que evolucionan las necesidades y los riesgos de seguridad de la organización. Regularmente se deberá revisar y actualizar estas políticas para asegurar que sigan siendo adecuadas y efectivas.
3.	Evaluar la implementación de autenticación multifactor (MFA) para accesos críticos.
Hacer:
	Implementar un servicio centralizado de autenticación como LDAP o Active Directory.
	Configurar y documentar la integración del servidor web y la base de datos con el servicio de autenticación centralizado.
	Establecer MFA para todas las cuentas de administradores y cuentas con acceso privilegiado.
Check:
	Verificar que todos los usuarios tengan acceso apropiado según sus roles y responsabilidades.
	Revisar la configuración de MFA para asegurar su efectividad y cumplimiento con las políticas establecidas.
Actuar:
	Corregir cualquier desviación encontrada durante las revisiones.
	Mejorar las políticas de gestión de identidades y MFA en base a las lecciones aprendidas y mejores prácticas.

Aspecto de Seguridad: Autorización
Objetivo 2: Reforzar el Control de Acceso y la Autorización
Planificar:
	Definir roles y permisos necesarios para acceder a recursos críticos.
	Implementar un sistema de control de acceso basado en roles (RBAC).
Hacer:
	Configurar listas de control de acceso (ACLs) en el sistema operativo y la base de datos para restringir el acceso a datos sensibles.
	Documentar y automatizar la revisión periódica de los permisos asignados.
Check:
	Realizar auditorías regulares para asegurar que los permisos asignados sigan siendo adecuados.
	Verificar que las ACLs estén correctamente configuradas y que no existan excepciones no autorizadas.
Actuar:
	Ajustar los permisos según cambios organizacionales o en los requisitos de seguridad.
	Implementar mejoras en los procedimientos de revisión y auditoría basados en los resultados obtenidos.


Checklist para Futuros Despliegues
Planificación:
¿Se ha documentado y comunicado claramente la política de gestión de identidades y autenticación?
¿Están definidos los roles y permisos requeridos para todos los recursos críticos?
Implementación (Hacer)
¿Se ha implementado correctamente el sistema de autenticación centralizado y MFA?
¿Están configuradas las ACLs y RBAC según las políticas establecidas?
Verificación (Check):
¿Se han realizado auditorías regulares de identidades y permisos?
¿Se han verificado y corregido las desviaciones encontradas durante las auditorías?
Acción (Actuar):
¿Se han ajustado los permisos y políticas según los cambios organizacionales o de seguridad?
¿Se han implementado mejoras en los procedimientos de revisión y auditoría?

Este programa PDCA asegura que el SGSI en Linux para las aplicaciones en la nube esté robustamente protegido, cumpla con las normativas y estándares de seguridad, y esté preparado para mantener la continuidad del negocio ante cualquier eventualidad.
