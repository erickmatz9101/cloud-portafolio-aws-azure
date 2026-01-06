Configuración inicial segura en AWS

 🎯 Objetivo
Configurar la cuenta AWS recién creada con buenas prácticas de seguridad y control de costos antes de iniciar los laboratorios.

 🛠️ Pasos realizados
1. Activé **MFA en el usuario root** para proteger el acceso principal.
2. Creé un **usuario IAM administrador** (`erick-admin`) y lo asigné al grupo `Administrators`.
3. Configuré **Billing Preferences** para recibir alertas de facturación y uso del Free Tier.
4. Definí un **budget de $5 USD** con alertas por correo.
5. Verifiqué los **$200 USD de créditos iniciales** disponibles.
6. Seleccioné la región por defecto (**us-east-1**) para mantener consistencia en los laboratorios.

 📸 Evidencias
<img width="1916" height="852" alt="1 -Billing preferences" src="https://github.com/user-attachments/assets/ce0eb6af-2402-4590-b755-428f1001b15c" />
 <img width="1912" height="866" alt="2 -Budgets" src="https://github.com/user-attachments/assets/85c11306-4b1d-447d-a24e-d3c5ff17b220" />
 <img width="1917" height="867" alt="3 -Credits" src="https://github.com/user-attachments/assets/742bbc5e-09ae-44cf-8f31-854f1ecf4337" />

 

🤔 Reflexión
Este paso inicial me permitió asegurar que mi entorno de práctica sea seguro y controlado.  
Aprendí la importancia de separar el usuario root de los usuarios de trabajo y de configurar alertas para evitar cargos inesperados.
