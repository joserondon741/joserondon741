# Jose Rafael Rondon Sosa
### Desarrollador Backend Trainee / Full Stack JavaScript

Bienvenido/a a mi portafolio profesional. Me especializo en el diseño e implementación de APIs RESTful escalables, arquitecturas modulares y desarrollo backend con Node.js, Express y bases de datos relacionales.

---

## 🛠️ Tecnologías y Herramientas

- **Lenguajes y Entornos:** JavaScript (ES6+), Node.js
- **Frameworks & Librerías:** Express.js, Sequelize ORM, dotenv, express-fileupload
- **Bases de Datos:** PostgreSQL, SQL
- **Seguridad & Autenticación:** JSON Web Tokens (JWT), Middlewares de Autorización Bearer, Hashing
- **Control de Versiones:** Git, GitHub
- **Pruebas y Documentación:** Thunder Client, Postman, cURL

---

## 🚀 Proyectos Destacados

### 1. Servidor Web Modular & Gestión de Logs (Módulo 6)
- **Tecnologías:** Node.js, Express, File System (`fs`), dotenv.
- **Descripción:** Servidor web estructurado con arquitectura modular (rutas y controladores), implementación de middlewares personalizados para auditoría de tráfico y registro de eventos en archivos planos (`log.txt`).
- **Enlace:** [Repositorio en GitHub](https://github.com/joserondon741/proyecto_modulo6-node-express)

### 2. API Transaccional con ORM & PostgreSQL (Módulo 7)
- **Tecnologías:** Node.js, Express, PostgreSQL, Sequelize ORM.
- **Descripción:** Capa de persistencia relacional con asociaciones 1:N entre entidades, operaciones CRUD completas, integridad referencial con eliminación en cascada (`CASCADE`) y control estricto de transacciones ACID mediante `ROLLBACK` automático ante excepciones.
- **Enlace:** [Repositorio en GitHub](https://github.com/joserondon741/proyecto-modulo7)

### 3. API RESTful Segura con JWT & Gestión de Archivos (Módulo 8)
- **Tecnologías:** Node.js, Express, Sequelize, PostgreSQL, JWT, express-fileupload.
- **Descripción:** API RESTful robusta protegida con autenticación sin estado mediante tokens JWT en cabeceras `Authorization: Bearer`, validación de roles en rutas privadas y procesamiento seguro de archivos multipart con listas blancas de extensiones y almacenamiento por marca temporal.
- **Enlace:** [Repositorio en GitHub](https://github.com/joserondon741/M-dulo-8---Autenticaci-n-JWT-y-Carga-de-Archivos-en-Express)

---

## 📌 Caso de Estudio Técnico: "Implementación de Arquitectura REST Segura con JWT y Gestión Controlada de Archivos"

- **Descripción de la actividad:**  
  Diseño y construcción de un sistema backend desacoplado para gestión de usuarios, autenticación y procesamiento de archivos multimedia, exponiendo endpoints REST normalizados bajo Node.js y Express.

- **Desafío principal:**  
  Garantizar el aislamiento estricto de rutas mutables (`PUT`, `DELETE`, `POST /upload`) sin comprometer el rendimiento del servidor, evitando el almacenamiento de sesiones en base de datos y mitigando riesgos de seguridad derivados de la inyección o saturación de disco por archivos no permitidos.

- **Solución propuesta:**  
  1. Adopción de autenticación sin estado (*stateless*) mediante tokens criptográficos **JWT** con tiempo de vida limitado y firma secreta.
  2. Implementación de un middleware interceptor (`authMiddleware`) para validar la integridad de la firma digital antes de dar paso a los controladores.
  3. Creación de una capa de subida de archivos con lista blanca de tipos MIME permitidos (`.jpg`, `.jpeg`, `.png`, `.pdf`) y renombrado automático mediante marcas temporales (*timestamps*) para impedir sobreescrituras en el servidor.

- **Herramientas técnicas utilizadas:**  
  Node.js, Express.js, PostgreSQL, Sequelize ORM, jsonwebtoken, express-fileupload, dotenv y Thunder Client.

- **Habilidades técnicas aplicadas:**  
  - Patrón de arquitectura MVC (Rutas, Controladores y Modelos).
  - Flujos de autenticación y autorización mediante cabeceras Bearer.
  - Manejo asíncrono y control centralizado de estados de respuesta HTTP (200, 201, 400, 401, 403, 500).
  - Manipulación y sanitización de datos multipart/form-data.

- **Métricas de impacto logradas:**  
  - **100% de aislamiento en rutas privadas:** Mitigación completa de accesos no autenticados en operaciones sensibles.
  - **0% de subidas arbitrarias:** Rechazo inmediato en servidor (HTTP 400) ante formatos no admitidos.
  - **Tiempos de latencia reducidos (< 50 ms):** Verificación ágil de firmas JWT en memoria sin consultas redundantes a la base de datos.

- **Justificación de elección:**  
  Este proyecto sintetiza el estándar moderno de la industria backend: integración entre persistencia relacional, seguridad criptográfica y diseño de servicios listos para ser consumidos por cualquier interfaz web o móvil.

---

## 📬 Contacto & Redes Profesionales

- **GitHub:** [github.com/joserondon741](https://github.com/joserondon741)
- **LinkedIn:** [linkedin.com/in/jose-rondon-sosa](https://www.linkedin.com)
