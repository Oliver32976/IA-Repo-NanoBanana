## Notas sobre el uso de herramientas

Las firmas de las herramientas se proporcionan automáticamente mediante llamadas a funciones.  
Este archivo documenta algunas restricciones y patrones de uso que no son evidentes.

### exec — Límites de seguridad

- Los comandos tienen un tiempo máximo de ejecución configurable (por defecto 60 segundos).
- Algunos comandos peligrosos están bloqueados para evitar daños al sistema.  
  Ejemplos: `rm -rf`, `format`, `dd`, `shutdown`, entre otros.
- La salida de los comandos se limita a un máximo de **10,000 caracteres**.
- La configuración `restrictToWorkspace` puede limitar el acceso a archivos únicamente dentro del espacio de trabajo del proyecto.

### cron — Recordatorios programados

Permite programar tareas o recordatorios automáticos en momentos específicos.

Para más información sobre su uso y configuración, consulta la documentación de la herramienta **cron**.