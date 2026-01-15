🎯 Objetivo

Diseñar una red virtual en AWS que permita separar recursos públicos y privados dentro de una misma VPC. Esta segmentación es clave para construir arquitecturas seguras, escalables y alineadas con buenas prácticas de infraestructura en la nube.

🔐 Beneficio

La separación entre subnets públicas y privadas permite:

Controlar el tráfico de red: solo los recursos públicos tienen acceso directo a Internet.

Reducir la superficie de ataque: los recursos privados (como bases de datos o servidores internos) permanecen aislados.

Facilitar la administración de seguridad: mediante reglas de routing, NAT y grupos de seguridad.

Preparar la infraestructura para alta disponibilidad: distribuyendo subnets en múltiples zonas de disponibilidad.

Evidencia:
<img width="1912" height="835" alt="VPC Creada" src="https://github.com/user-attachments/assets/fb4f6800-9f87-4d3d-ae06-16cd747b48d2" />
<img width="1916" height="652" alt="subnets publicas y privadas" src="https://github.com/user-attachments/assets/9bc7411b-a9c6-4f48-873b-bd9ac3921a6b" />
<img width="1912" height="678" alt="creando las route tables" src="https://github.com/user-attachments/assets/5204f21e-f693-4ff3-b4e4-a4f583a9a12f" />
<img width="1918" height="435" alt="creando internet gateway" src="https://github.com/user-attachments/assets/524b8c50-0607-47d4-b3ce-5f82c2c5c816" />
<img width="1918" height="436" alt="adjuntando IGW a VPV" src="https://github.com/user-attachments/assets/be47114b-60fd-4a51-a16d-7df57d1fd42b" />
<img width="1918" height="716" alt="creando y asociando a la RT privada " src="https://github.com/user-attachments/assets/2f47a065-ba83-4bc9-8080-a9f79f5670f7" />

🧠 Reflexión técnica

Este diseño es una base sólida para arquitecturas más complejas como:

Aplicaciones web con frontend en subnets públicas y backend en privadas.

Bases de datos protegidas que solo responden a instancias internas.

Infraestructura escalable con balanceadores, NAT, y firewalls.

Separar recursos públicos y privados no solo es una práctica recomendada, sino una necesidad para entornos productivos que requieren seguridad, trazabilidad y control granular del tráfico.
