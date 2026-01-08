🎯 Objetivo
Levantar una instancia EC2 t2.micro  dentro del Free Tier de AWS y reflexionar sobre los beneficios, riesgos y buenas prácticas al usar este servicio.

🚀 Beneficios de Amazon EC2
Escalabilidad inmediata: lanzar servidores en minutos, sin necesidad de hardware físico.

Flexibilidad total: elegir sistema operativo, tamaño de instancia y red según la necesidad del proyecto.

Modelo de pago por uso: solo consumes lo que necesitas, ideal para pruebas y entornos productivos.

Integración con otros servicios AWS: conexión sencilla con S3, RDS, Lambda, etc.

Free Tier: oportunidad de aprender y experimentar sin costo inicial.

⚠️ Riesgos y cómo mitigarlos
Acceso no autorizado (SSH abierto a todo el mundo)  
🔒 Mitigación: limitar el puerto 22 solo a tu IP en el Security Group.

Costos inesperados fuera del Free Tier  
💰 Mitigación: configurar alertas de facturación y monitorear con AWS Budgets.

Exposición de claves privadas (.pem)  
🔑 Mitigación: guardar el archivo en un lugar seguro, nunca subirlo a GitHub ni compartirlo.

Instancias olvidadas en estado Running  
⏹️ Mitigación: detener o terminar instancias cuando no se usen.

Puertos abiertos innecesarios (HTTP/HTTPS sin configuración)  
🛡️ Mitigación: abrir solo los puertos necesarios y aplicar reglas de firewall estrictas.

📸 Evidencias:
<img width="1887" height="806" alt="Security Groups" src="https://github.com/user-attachments/assets/969427c4-59c6-4813-97dc-345e16030bca" />
<img width="1896" height="532" alt="key pair" src="https://github.com/user-attachments/assets/bc9297e5-b7a2-4d7b-a3b4-6e0de2136341" />
<img width="1898" height="817" alt="Instancia Runing" src="https://github.com/user-attachments/assets/9d2e9a6b-d40b-4750-83f3-e970d90c651a" />
<img width="1448" height="625" alt="Conexion EC2" src="https://github.com/user-attachments/assets/ca085ab2-f3c7-4c57-a2bb-f1ddfbeabce9" />




💡 Reflexión
Más allá de la ejecución técnica, EC2 representa una puerta de entrada a la infraestructura moderna: flexible, escalable y segura si se usa con criterio. Documentar beneficios y riesgos me permite construir un portafolio que no solo muestra ejecución técnica, sino también visión profesional sobre seguridad, costos y buenas prácticas en la nube.
