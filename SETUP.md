\# 🚀 Setup del Proyecto - LetRob Market



\## Requisitos Previos



\- \[Docker Desktop](https://www.docker.com/products/docker-desktop/) instalado

\- \[Node.js 20+](https://nodejs.org/) (opcional)

\- \[Git](https://git-scm.com/)

\- \[Angular CLI](https://angular.io/cli): `npm install -g @angular/cli`



\## 📥 Clonar el Repositorio

```bash

git clone https://github.com/robert-agustin/LetRob\_Market.git

cd LetRob-Market

```



\## 🔧 Configuración del Backend



\### 1. Configurar variables de entorno

```bash

cd backend

cp .env.example .env

```



El archivo `.env` ya está configurado para Docker. No necesitas modificarlo.



\### 2. Levantar servicios con Docker

```bash

\# Volver a la raíz

cd ..



\# Levantar PostgreSQL + Backend

docker compose up

```



Espera a ver:

```

✅ Conexión a PostgreSQL exitosa

🚀 Servidor corriendo en http://localhost:3000

```



\### 3. Verificar



Abre: http://localhost:3000



\## 🎨 Configuración del Frontend (Angular)



\### 1. Crear proyecto Angular

```bash

\# Desde la raíz del proyecto

ng new frontend --routing --style=scss



\# Opciones:

\# ✅ Would you like to add Angular routing? → Yes

\# ✅ Which stylesheet format? → SCSS

```



\### 2. Instalar Angular Material

```bash

cd frontend

ng add @angular/material

```



\### 3. Levantar frontend

```bash

ng serve

\# o

npm start

```



Frontend: http://localhost:4200



\## 🐳 Comandos Docker Útiles

```bash

\# Levantar

docker compose up



\# Segundo plano

docker compose up -d



\# Ver logs

docker compose logs -f backend



\# Detener

docker compose down



\# Reiniciar backend

docker compose restart backend

```



\## 🌿 Flujo Git

```bash

\# Trabajar en develop

git checkout develop

git pull origin develop



\# Hacer cambios

git add .

git commit -m "feat: descripción"

git push origin develop

```



\## 📂 Estructura

```

LetRob-Market/

├── backend/         ← Express + PostgreSQL

├── frontend/        ← Angular (por crear)

├── docker-compose.yml

└── README.md

```



\## 🆘 Problemas Comunes



\*\*Puerto 5432 ocupado:\*\* Ya está configurado en 5433



\*\*Docker no corre:\*\* Abre Docker Desktop



\*\*No conecta a DB:\*\*

```bash

docker compose down

docker compose up

```



\## ✅ Checklist



\- \[ ] Docker Desktop corriendo

\- \[ ] Repo clonado

\- \[ ] `docker compose up` funcionando

\- \[ ] Backend en http://localhost:3000

\- \[ ] Frontend creado con Angular

\- \[ ] Frontend en http://localhost:4200

