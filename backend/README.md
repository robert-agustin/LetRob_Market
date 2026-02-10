\# Backend - LetRob Market



API REST para e-commerce de productos digitales.



\## 🚀 Desarrollo



\### Con Docker (recomendado)

```bash

\# Desde la raíz del proyecto

docker compose up

```



\### Sin Docker

```bash

\# Instalar dependencias

npm install



\# Configurar .env

cp .env.example .env



\# Levantar servidor de desarrollo

npm run dev

```



\## 📚 Dependencias



\- express - Framework web

\- sequelize - ORM

\- pg - Cliente PostgreSQL

\- bcryptjs - Encriptación de contraseñas

\- jsonwebtoken - Autenticación JWT

\- dotenv - Variables de entorno

\- cors - CORS

\- express-validator - Validación de datos



\## 🗂️ Estructura

```

src/

├── config/       # Configuraciones

├── controllers/  # Controladores

├── models/       # Modelos Sequelize

├── routes/       # Rutas

├── middlewares/  # Middlewares

├── services/     # Servicios externos

├── utils/        # Utilidades

└── server.js     # Punto de entrada

```



\## 🔑 Variables de Entorno



Ver `.env.example` para la lista completa.

