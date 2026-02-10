\# 🛒 LetRob Market - E-commerce de Productos Digitales



Plataforma de comercio electrónico para venta de productos digitales (ebooks, cursos, plantillas).



\## 🚀 Stack Tecnológico



\### Backend

\- Node.js 20

\- Express.js

\- PostgreSQL 15

\- Sequelize ORM

\- JWT Authentication



\### Frontend (próximamente)

\- Angular 17+

\- Angular Material



\### DevOps

\- Docker \& Docker Compose



\## 📋 Requisitos Previos



\- Docker Desktop

\- Node.js 20+ (opcional, si quieres correr sin Docker)

\- Git



\## 🔧 Instalación y Configuración



\### 1. Clonar el repositorio

```bash

git clone <url-del-repo>

cd LetRob\_Market

```



\### 2. Configurar variables de entorno

```bash

cd backend

cp .env.example .env

\# Editar .env con tus configuraciones

```



\### 3. Levantar con Docker

```bash

\# Desde la raíz del proyecto

docker compose up --build

```



El backend estará disponible en: http://localhost:3000

PostgreSQL estará disponible en: localhost:5433



\### 4. Verificar que funciona



Abre tu navegador: http://localhost:3000



Deberías ver:

```json

{

&nbsp; "message": "🚀 API de E-commerce funcionando",

&nbsp; "version": "1.0.0"

}

```



\## 📁 Estructura del Proyecto

```

LetRob\_Market/

├── backend/

│   ├── src/

│   │   ├── config/         # Configuraciones (BD, JWT, etc)

│   │   ├── controllers/    # Lógica de negocio

│   │   ├── models/         # Modelos de Sequelize

│   │   ├── routes/         # Rutas de la API

│   │   ├── middlewares/    # Middlewares (auth, validación)

│   │   ├── services/       # Servicios (email, pagos, storage)

│   │   ├── utils/          # Utilidades

│   │   └── server.js       # Entrada principal

│   ├── .env                # Variables de entorno (NO subir a Git)

│   ├── .env.example        # Plantilla de .env

│   ├── Dockerfile

│   └── package.json

├── frontend/               # (Pendiente)

├── docker-compose.yml

├── .gitignore

└── README.md

```



\## 🐳 Comandos de Docker

```bash

\# Levantar servicios

docker compose up



\# Levantar en segundo plano

docker compose up -d



\# Ver logs

docker compose logs -f



\# Ver logs solo del backend

docker compose logs -f backend



\# Detener servicios

docker compose down



\# Detener y eliminar volúmenes (⚠️ borra la BD)

docker compose down -v



\# Reiniciar solo el backend

docker compose restart backend



\# Entrar al contenedor del backend

docker exec -it ecommerce\_backend sh



\# Entrar a PostgreSQL

docker exec -it ecommerce\_postgres psql -U admin -d ecommerce\_dev

```



\## 🔒 Endpoints de la API



\### Públicos

\- `GET /` - Información de la API

\- `GET /health` - Health check



\### Autenticación (próximamente)

\- `POST /api/auth/register` - Registro de usuarios

\- `POST /api/auth/login` - Login

\- `POST /api/auth/logout` - Logout



\### Productos (próximamente)

\- `GET /api/products` - Listar productos

\- `GET /api/products/:slug` - Detalle de producto

\- `POST /api/products` - Crear producto (admin)



\### Carrito (próximamente)

\- `GET /api/cart` - Ver carrito

\- `POST /api/cart/add` - Agregar al carrito

\- `DELETE /api/cart/remove/:id` - Eliminar del carrito



\## 👥 Equipo de Desarrollo



\- Developer 1 - Backend

\- Developer 2 - Frontend



\## 📝 Notas de Desarrollo



\### Variables de Entorno

\- Nunca subir `.env` a Git

\- Usar `.env.example` como plantilla

\- Cada desarrollador tiene su propio `.env`



\### Git Workflow

\- `main` - Producción

\- `develop` - Desarrollo

\- `feature/\*` - Nuevas funcionalidades



\### Commits

Usar convención de commits:

\- `feat:` - Nueva funcionalidad

\- `fix:` - Corrección de bugs

\- `docs:` - Documentación

\- `refactor:` - Refactorización



\## 🔜 Próximos Pasos



\- \[ ] Sistema de autenticación (JWT)

\- \[ ] CRUD de productos

\- \[ ] Sistema de carrito

\- \[ ] Integración de pagos

\- \[ ] Sistema de descargas

\- \[ ] Frontend con Angular



\## 📄 Licencia



Este proyecto es privado y confidencial.

