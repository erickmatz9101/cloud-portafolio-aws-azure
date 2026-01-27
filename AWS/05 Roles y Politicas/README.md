# 🚀 Práctica 6: IAM Roles y Políticas

## 🎯 Objetivo
Configurar un IAM Role que permita a una instancia EC2 acceder a un bucket S3 de forma segura y controlada, aplicando el principio de menor privilegio.

## 💡 Racional
En arquitecturas cloud, los servicios deben interactuar sin compartir credenciales explícitas. IAM Roles permiten delegar permisos de forma segura, escalable y auditable. Esta práctica demuestra cómo EC2 puede acceder a S3 mediante un rol con permisos definidos.

## ✅ Beneficios
- 🔒 Seguridad reforzada al evitar credenciales hardcoded.  
- 📈 Escalabilidad: el mismo rol puede aplicarse a múltiples instancias.  
- 📝 Auditoría clara de accesos y permisos.  
- 🧩 Modularidad: roles y políticas se pueden versionar y reutilizar.  

## ⚠️ Riesgos
- 🚨 Políticas demasiado amplias pueden exponer recursos sensibles.  
- ❌ Asociación incorrecta del rol puede impedir el acceso esperado.  
- 🔍 Falta de validación puede generar errores silenciosos en producción.  

## 📸 Evidencia
<img width="1897" height="713" alt="creando roles" src="https://github.com/user-attachments/assets/cdcbf95a-c0cb-4e43-82c2-a74cc3889b4a" />
<img width="1907" height="587" alt="seleccionado las politicas" src="https://github.com/user-attachments/assets/97bb78f6-ca99-4f11-a657-a613f030aef9" />
<img width="1892" height="813" alt="adjuntando politicas y rol" src="https://github.com/user-attachments/assets/f27e542e-1ba6-4a76-bdda-8ce93b5b3bcf" />
<img width="1910" height="662" alt="asociando el rol a la instancia EC2" src="https://github.com/user-attachments/assets/83cb14fe-71b9-4637-bfeb-cecf49505754" />
<img width="1206" height="677" alt="validando conexion por medio de roles" src="https://github.com/user-attachments/assets/e17e0744-64ad-4a16-a9ca-eb9c16d6ee48" />

### 🔹 Rol creado
- 🏷️ Nombre: `EC2-S3-ReadRole`  
- 🛠️ Tipo: AWS Service → EC2  
- 📜 Política adjunta: `AmazonS3ReadOnlyAccess`  
