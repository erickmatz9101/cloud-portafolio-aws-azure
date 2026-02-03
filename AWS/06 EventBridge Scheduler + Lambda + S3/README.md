Práctica 6: EventBridge Scheduler + Lambda + S3
🎯 Objetivo  
Configurar un EventBridge Scheduler en AWS para invocar una función Lambda que genera archivos en S3, validando tanto ejecuciones únicas (One-time) como recurrentes (Rate-based).

💡 Por qué hacerlo  
La automatización en la nube no depende solo de levantar funciones o buckets, sino de orquestar servicios que trabajen juntos. EventBridge Scheduler permite programar tareas sin intervención manual, asegurando que procesos críticos se ejecuten en el momento adecuado y con la frecuencia necesaria.

✅ Beneficios  
⚡ Automatización de tareas sin necesidad de cron jobs externos.
📂 Evidencia clara en S3 de ejecuciones programadas.
🔄 Flexibilidad para configurar ejecuciones únicas o recurrentes.
🛠️ Integración nativa con Lambda y otros servicios de AWS.

⚠️ Riesgos o amenazas de no hacerlo  
⏱️ Ejecuciones críticas que dependen de intervención manual.
🚫 Posibles fallos por errores humanos en horarios o repeticiones.
💸 Costos innecesarios si los schedules no se detienen tras pruebas.
🔐 Falta de control en permisos IAM, impidiendo que los servicios se invoquen correctamente.

📸 Evidencias  
<img width="1915" height="707" alt="01 Generando S3" src="https://github.com/user-attachments/assets/9fdc68ac-83dc-47a5-82fe-576b90466a2f" />
<img width="1902" height="852" alt="02 Creando la función lambda" src="https://github.com/user-attachments/assets/755549f6-2e85-4f18-a38c-14067aafcef7" />
<img width="1912" height="847" alt="03 Agregando los permisos a S3 mediante IAM" src="https://github.com/user-attachments/assets/39a041ba-7643-4f96-8edd-d670e5e53b07" />
<img width="1912" height="827" alt="04 generando el test para validar que funcione" src="https://github.com/user-attachments/assets/b0f0d76d-ee00-4d6d-9bac-92248b708dbd" />
<img width="1886" height="791" alt="05 validando que la funcion lambda corra de forma correcta" src="https://github.com/user-attachments/assets/79d04e7d-a827-4dd9-9dc5-c44b8ecafe3e" />
<img width="1905" height="543" alt="06 verificando que el objeto este en S3" src="https://github.com/user-attachments/assets/c8b82eca-9229-458e-bc1d-7f11b2aa92ad" />
<img width="1907" height="982" alt="07 generando evento en  EventBridge para genenar el objeto de forma automática y periódicamente" src="https://github.com/user-attachments/assets/eaf41801-fa4c-414b-8eb8-c9b43797e594" />
<img width="1470" height="448" alt="08 generando la prueba" src="https://github.com/user-attachments/assets/b1976171-780f-412c-8505-c78a6f974a1a" />
<img width="1606" height="806" alt="09 Configurtacion final para que se genere el evento " src="https://github.com/user-attachments/assets/67f4bb93-2793-42cb-9fe5-c96a95b28dd4" />
<img width="1915" height="792" alt="10 validacion de la creacion periódica de los txt mediante el trigger" src="https://github.com/user-attachments/assets/a15ad945-3790-4004-810b-347e0e0a0ac4" />


🤔 Reflexión  
La práctica demuestra que automatizar en AWS no es solo cuestión de configurar servicios, sino de entender sus dependencias invisibles: tiempo, permisos, costos y validación.
El error de IAM enseñó que los roles no solo necesitan permisos, sino también relaciones de confianza para que otros servicios los asuman.
Más allá de la ejecución técnica, esta experiencia refuerza que cada detalle —desde la hora exacta hasta la política de confianza— impacta directamente en la confiabilidad y eficiencia de la infraestructura.
